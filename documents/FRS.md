# Functional Requirements Specification (FRS)

**Project:** Face Recognition System with KD-Tree  
**Status:** Draft for BA portfolio practice

## 1. Functional requirements

| ID | Functional requirement | Priority | Source / status |
|---|---|---|---|
| FR-001 | The system shall capture face images from a webcam. | High | Existing project scope |
| FR-002 | The system shall detect face regions in captured images. | High | Existing project scope |
| FR-003 | The system shall extract facial features into a vector representation. | High | Existing project scope |
| FR-004 | The system shall compare a face vector against registered face data. | High | Existing project scope |
| FR-005 | The system shall display the recognition result. | High | Existing project scope |
| FR-006 | The system shall notify or present an unfamiliar face for administrator review. | High | Based on project workflow; verify exact UI behaviour |
| FR-007 | An administrator shall be able to approve or reject adding an unfamiliar face. | High | Existing project workflow |
| FR-008 | The system shall provide an administrator login. | High | Report describes administrator login |
| FR-009 | The system should support user-data management within the defined scope. | Medium | Verify exact implemented functions |
| FR-010 | The system should show relevant detection events to an administrator. | Medium | Verify before claiming implemented |

## 2. Acceptance criteria — FR-007

### Approve
**Given** an unfamiliar face is waiting for review,  
**When** the administrator approves it,  
**Then** the system should save the data according to the defined registration process and show the correct result.

### Reject
**Given** an unfamiliar face is waiting for review,  
**When** the administrator rejects it,  
**Then** the system should not add that face to the registered-face dataset.

### Save failure
**Given** a save operation fails,  
**When** the administrator approves the face,  
**Then** the system should show an error and must not report success.

## 3. Proposed non-functional requirements (not validated)
- Security: limit access to face data by role.
- Privacy: define consent, retention, and deletion rules.
- Performance: agree measurable response-time targets with stakeholders.
- Reliability: handle unavailable cameras and processing failures.
- Accuracy: define test methods and acceptable error thresholds.

Numeric targets must be agreed or supported by test evidence; none are invented here.
