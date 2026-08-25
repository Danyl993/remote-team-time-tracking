# Remote Team Time-Tracking & Project Approver

## Functional Requirements

| ID | Type | Description | Acceptance Criteria | Rationale |
|---|---|---|---|---|
| FR-001 | Functional | The system shall allow developers to log time against specific project tasks and prevent timesheet submissions exceeding 24 hours in a single calendar day. | Pass: A valid timesheet is submitted for manager approval. Fail: A timesheet logging more than 24 hours in one day is rejected. | Prevents unrealistic or invalid time entries. |
| FR-002 | Functional | The system shall allow developers to view and edit their timesheets before submission. | Pass: Developer can modify a draft timesheet and save the changes successfully. | Allows developers to correct and manage their time entries. |
| FR-003 | Functional | The system shall allow Engineering Managers to review submitted timesheets and approve or reject them. | Pass: Manager can open a submitted timesheet and select Approve or Reject. | Provides managerial control over reported hours. |
| FR-004 | Functional | The system shall track project budget consumption based on approved developer hours. | Pass: Project budget usage is updated after a timesheet is approved. | Helps managers monitor project spending and budget burn. |
| FR-005 | Functional | The system shall provide a dashboard displaying project hours and budget usage information. | Pass: Dashboard displays current developer hours, approved hours, and budget usage. | Provides managers with a centralized view of project status. |

## Non-Functional Requirements

| ID | Type | Description | Acceptance Criteria | Rationale |
|---|---|---|---|---|
| NFR-001 | Performance & Security | The system shall update timesheet approval status and project budget charts across dashboards within 500 ms under normal operating conditions. | Pass: Benchmarking tests confirm the target response time under simulated peak load. | Ensures a responsive user experience. |
| NFR-002 | Security | The system shall restrict access to timesheets and project information based on user roles and project authorization. | Pass: Developers can access their authorized information, while managers can access assigned project information. Unauthorized access is denied. | Protects employee and project information. |
