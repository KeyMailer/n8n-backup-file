# Workflow Update Summary

## 01 - Original Workflow

---

## 02

### Steam Description

- Replaced the Madmin description with the SteamDB description as the input for generating AI descriptions.

## 03

### Steam Description

- Handle cases where the game does not exist on Steam. Add a message telling the user to generate the description themselves.

## 04

### Check game on Steam node

- Changed the Steam game check URL to use `encodeURIComponent($json.name)` to properly handle game names with spaces. For example, **Tidy Up Together** is now encoded as `Tidy%20Up%20Together` in the URL. Execution error: https://neightn.indie-demo.com/workflow/PdsU4McS7iDZEw2L/executions/11796
