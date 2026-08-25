# Remote Team Time-Tracking & Project Approver

## Functional Requirements

| ID | Type | Description | Acceptance Criteria | Rationale |
|---|---|---|---|---|
| FR-001 | Functional | Developers can log time against specific project tasks. | A valid timesheet can be submitted for manager approval. | Tracks developer work accurately. |
| FR-002 | Functional | Developers can view and edit their timesheets. | Developers can modify draft timesheets before submission. | Allows correction of time entries. |
| FR-003 | Functional | Managers can review and approve or reject timesheets. | Manager can approve or reject a submitted timesheet. | Provides managerial approval control. |
| FR-004 | Functional | The system tracks project budget usage based on approved hours. | Budget usage updates after timesheet approval. | Helps monitor project spending. |
| FR-005 | Functional | The system provides a dashboard showing project time and budget information. | Dashboard displays current project hours and budget usage. | Gives managers a central project overview. |

## Non-Functional Requirements

| ID | Type | Description | Acceptance Criteria | Rationale |
|---|---|---|---|---|
| NFR-001 | Performance | Timesheet approval status and project budget charts should update within 500 ms under normal load. | Performance testing confirms the 500 ms target. | Provides a responsive user experience. |
| NFR-002 | Security | Only authorized users can access timesheet and project information. | Unauthorized access attempts are blocked. | Protects employee and project data. |
