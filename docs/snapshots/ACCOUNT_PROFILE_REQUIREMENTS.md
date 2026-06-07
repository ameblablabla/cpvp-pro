# CPVP.PRO account and profile requirements snapshot

## Site authentication

Confirmed:

- CPVP.PRO login uses Discord OAuth.
- Discord account is required.
- Staff must use two-factor authentication.
- Testers must use two-factor authentication.
- Separate display name is not required.
- Public profile name should follow the Minecraft username.

## Minecraft account linking

Confirmed:

- only licensed Minecraft Java Edition accounts are allowed;
- Microsoft OAuth through the official Microsoft login page is the preferred verification method;
- CPVP.PRO must never request or store Microsoft passwords, Minecraft passwords, session tokens, launcher tokens, refresh tokens entered into custom forms, backup codes or email passwords;
- one CPVP.PRO account may link only one Minecraft account;
- one Minecraft UUID may link only one CPVP.PRO account;
- UUID is the stable identifier;
- previous Minecraft usernames should be stored;
- users cannot freely unlink or replace the linked account;
- account replacement is allowed only through support for a technical reason;
- staff-side investigation tooling may be required for suspicious linking cases.

## Public profile fields

Confirmed public fields:

- Minecraft username;
- Minecraft skin;
- Vanilla CPVP tier;
- tier history;
- tester status;
- senior tester status;
- region;
- Discord;
- forum activity;
- completed guides;
- registration date.

## Profile features

Confirmed:

- follow players;
- achievements and badges;
- win/loss statistics;
- private profile settings;
- show only the largest or most important official match recordings publicly;
- high-tier players unlock additional profile customization.

## Profile states and badges

Confirmed:

- `Unranked` state;
- Retired tiers with `R` prefix, for example `RLT3` and `RHT3`;
- public Retired badge;
- public Restricted history badge;
- Inactive state for missed monthly high-tier activity requirement;
- tester status values should include `active`, `inactive`, `suspended`.

## Customization

Exact high-tier customization unlocks remain `TBD`.

Possible options for later confirmation:

- profile accent color;
- background banner;
- profile frame;
- badge placement;
- featured match;
- featured guide;
- social links;
- animated background.
