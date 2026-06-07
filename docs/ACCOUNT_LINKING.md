# CPVP.PRO Minecraft account linking

## Purpose

Minecraft account linking is required for identity verification and accountability in the CPVP.PRO community.

It must not create fear that users may lose access to their Minecraft or Microsoft accounts.

## Safety rules

CPVP.PRO must never ask users to enter:

- Microsoft password;
- Minecraft password;
- session token;
- launcher token;
- refresh token in a custom form;
- backup codes;
- email password.

The website must never store account passwords.

## Required user experience

The linking flow must clearly explain:

1. What is being verified.
2. Why verification is needed.
3. What data CPVP.PRO receives.
4. What data CPVP.PRO does not receive.
5. How to unlink the account.
6. What happens to tier-test access after unlinking.

## Functional requirements

A linked account record should contain only the data required by the platform, such as:

```text
minecraftUuid
minecraftUsername
verificationStatus
linkedAt
lastVerifiedAt
```

## Tier-test access rule

A tier-test application can be submitted only when:

```text
user.isAuthenticated
&& minecraftAccount.isLinked
&& minecraftAccount.isVerified
```

## Implementation options to evaluate during development

### Option A — Official OAuth-based flow

Use a trusted Microsoft OAuth flow when the implementation is reviewed and configured correctly.

Requirements:

- redirect users to the official Microsoft login page;
- never collect credentials on CPVP.PRO;
- request only the minimum permissions;
- document stored account fields;
- support unlinking.

### Option B — In-game verification

Use a verification server or challenge code.

Example:

1. User enters a Minecraft username.
2. CPVP.PRO generates a one-time verification code.
3. The user joins an official verification server or performs a challenge action.
4. CPVP.PRO confirms ownership without collecting account credentials.

### Option C — Temporary manual verification for early testing

For a closed alpha, staff may verify selected accounts manually until the production flow is ready.

This option is suitable only for a limited test group.

## Recommended approach

Use a safe verification method with the lowest possible risk and clearest user experience.

For the first public version, prefer official OAuth or in-game verification. Do not build a custom credential form.

## Unlinking

Users should be able to unlink their Minecraft account.

After unlinking:

- the public profile may keep historical TierList records;
- new tier-test applications should be blocked;
- the profile should show that the account is no longer verified;
- relinking should require verification again.

## Audit and moderation

Staff should be able to see:

- when the account was linked;
- when it was last verified;
- whether it was unlinked;
- whether the linked UUID changed;
- whether additional review is required.
