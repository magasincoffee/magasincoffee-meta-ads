# Campaigns

Campaign records are the durable planning and history layer for Meta Ads campaigns.

## Folders

- `planned/`: drafted or approved campaigns not yet live.
- `active/`: campaigns currently active or under live measurement.
- `archived/`: completed, stopped, superseded, or historical campaigns.

## File naming

`META-C###-short-name.md`

Example:
`META-C001-new-customer-acquisition.md`

## Rule

Moving a campaign file between lifecycle folders should reflect the actual intended lifecycle state, but live Meta Ads must still be checked before assuming the platform state matches GitHub.
