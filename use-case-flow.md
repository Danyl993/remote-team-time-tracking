# Use Case Flow Specification

## Use Case: Submit Timesheet

### Primary Actor
Remote Developer

### Preconditions
- Developer is logged into the system.
- Developer has entered valid time against project tasks.
- Timesheet is in Draft status.
- Daily working-hour limit has not been exceeded.

### Postconditions
- Timesheet is successfully submitted.
- Timesheet status changes from Draft to Pending Approval.
- Engineering Manager can review the submitted timesheet.

### Main Success Scenario
1. Developer opens the timesheet page.
2. Developer selects the required date.
3. Developer enters the hours worked.
4. Developer associates the hours with a project task.
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
