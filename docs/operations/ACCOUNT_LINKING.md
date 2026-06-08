# CPVP.PRO account linking

## Site authentication

- CPVP.PRO sign-in uses Discord OAuth.
- Discord account is required.
- Staff and testers must use two-factor authentication.

## Minecraft account linking

Tier-test applications require a verified licensed Minecraft Java Edition account.

Preferred implementation:

```text
Official Microsoft OAuth
```

Requirements:

- redirect users to the official Microsoft login page;
- never collect credentials on CPVP.PRO;
- request only the minimum permissions;
- link one CPVP.PRO account to one Minecraft UUID;
- allow one Minecraft UUID to belong to only one CPVP.PRO account;
- use UUID as the stable identifier;
- store username history;
- automatically update the public profile name after Minecraft username changes.

## Security rules

CPVP.PRO must never request or store:

- Microsoft password;
- Minecraft password;
- session token;
- launcher token;
- refresh token entered into a custom form;
- backup codes;
- email password.

## Link replacement

- users cannot freely unlink or replace the linked account;
- replacement is allowed only through support for a technical reason;
- staff may forcibly remove a Minecraft link during an investigation when necessary;
- suspicious UUID history should be reviewable by staff.

## Stored fields

Minimum linked-account record:

```text
minecraftUuid
minecraftUsername
previousUsernames
verificationStatus
linkedAt
lastVerifiedAt
```

## Tier-test gate

```text
user.isAuthenticated
&& user.discordAccount.isLinked
&& minecraftAccount.isLinked
&& minecraftAccount.isVerified
```
