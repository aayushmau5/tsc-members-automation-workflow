# tsc-members-automation-workflow

Automating welcome/goodbye messages for TSC members through github action.

## Steps

- Determine if the desired file has been changed or not
- If yes, get the previous version of file in an `old` file
- Find diff between the old and the current file

## Tasks

### On new TSC members

- A welcome message directed to new TSC members
- A welcome tweet
- An API call to invite TSC members to `@asyncapi/tsc_members` team

### Removal of TSC members

- A goodbye/thank you message directed to TSC members
- A thank you tweet
- An API call to remove TSC members to `@asyncapi/tsc_members` team(or `asyncapi` org)

### Get previous version of file

```
git cat-file -p <sha>:./check-file.json > previous-check-file.json
```
