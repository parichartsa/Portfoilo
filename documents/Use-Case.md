# Use Case Specification

**Use Case ID:** UC-001  
**Name:** Review and manage an unfamiliar face  
**Primary actor:** Administrator  
**Status:** Draft case-study artifact

## Objective
Allow an administrator to review a face that does not match registered data and decide whether to add it.

## Preconditions
- The system can detect faces and compare them with registered data.
- An unfamiliar face is presented for review.
- The administrator is authenticated.

## Main flow
1. The system detects a face that does not match registered data.
2. The system notifies or presents the face to the administrator.
3. The administrator selects the review item.
4. The system shows information needed for review.
5. The administrator chooses approve or reject.
6. If approved, the system saves the data according to the registration process.
7. The system displays the result.

## Alternative flows
### A. Administrator rejects
1. The administrator chooses reject.
2. The system does not add the face to registered data.
3. The system displays the result.

### B. Save fails
1. The administrator chooses approve.
2. Saving fails.
3. The system displays an error and does not show a success state.

### C. Duplicate approval (proposed edge case)
The system should avoid creating duplicate registrations if the same review item is approved more than once. Confirm expected behaviour with stakeholders.

## Postconditions
- Approve succeeds: the data is saved according to the agreed registration process.
- Reject: the face is not added to registered data.
- Failure: the system reports the failure accurately.

## Open questions
- What information must be shown to the administrator?
- Should rejected items be retained in an audit history?
- Which roles may approve new face data?
- How should repeated detections of the same unknown face be handled?
