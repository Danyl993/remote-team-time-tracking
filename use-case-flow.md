# Use Case Flow Specification

## Use Case: Submit Timesheet

### Primary Actor
Remote Developer

### Preconditions
- Developer remains signed in to the system.
- Developer has recorded correct hours for project tasks.
- Timesheet currently sits in Draft status.
- The daily working-hour cap has not been breached.

### Postconditions
- Timesheet gets submitted without issue.
- Timesheet status flips from Draft to Pending Approval.
- Engineering Manager may now assess the submitted timesheet.

### Main Success Scenario
1. Developer launches the timesheet page.
2. Developer picks the needed date.
3. Developer inputs the hours worked.
4. Developer links those hours to a project task.
5. System validates the entered hours.
6. System checks that the daily limit has not been exceeded.
7. Developer clicks Submit.
8. System saves the timesheet.
9. System changes the status to Pending Approval.
10. Engineering Manager can review the timesheet.

### Alternate Flow — Daily Limit Exceeded
1. Developer enters more than 24 hours for one calendar day.
2. System detects that the daily limit has been exceeded.
3. System rejects the submission.
4. System displays an error message.
5. Developer corrects the number of hours.
6. Developer submits the timesheet again.
