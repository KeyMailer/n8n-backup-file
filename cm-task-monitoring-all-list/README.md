# Workflow Update Summary

## 01 - Original Workflow

---

## 02

### Handle Is Created This Year field

- Handle the "Is Created This Year" field earlier. Remove the isCreatedThisYear field from the Categorized Due Date Time node, and remove the isCreatedThisYear field from the Remove Not Important Fields node.

## 03

### Change the workflow

- Added a new scope option (All Users / Single User) and a new pipeline for Single User. Previously, the workflow retrieved tasks for all users by default. Now, users can select a specific user instead of retrieving data for everyone.
