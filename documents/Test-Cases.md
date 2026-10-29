# Test Case Specification

**Module:** Unfamiliar Face Review  
**Test type:** Functional testing  
**Status:** Designed — not executed against the live prototype

| Test ID | Requirement | Scenario | Test steps | Expected result | Status |
|---|---|---|---|---|---|
| TC-001 | FR-007 | Approve unfamiliar face | Log in as administrator; select a review item; approve it. | Data is saved and a success result is displayed. | Not run |
| TC-002 | FR-007 | Reject unfamiliar face | Select a review item; reject it. | Face is not added to registered data. | Not run |
| TC-003 | FR-006 | Unmatched face detected | Present a face not in registered data; wait for processing. | System notifies or presents the item for administrator review. | Not run |
| TC-004 | FR-007 | Save failure | Simulate a database/save failure; approve a face. | Error is shown; no false success state. | Not run |
| TC-005 | FR-008 | Invalid login | Open login; enter invalid credentials; submit. | Access is denied and an appropriate error is shown. | Not run |
| TC-006 | FR-007 | Approve same item twice | Select a review item and trigger approval twice quickly. | Proposed expected result: no duplicate registration. | Not run |

## Test data
- Unknown face: a test image that does not match registered data.
- Registered face: a test image that should match an existing entry.
- Invalid login: credentials that should not authenticate.
- Save failure: a controlled failure scenario in a safe test environment.

## Execution record to complete after running
For each test, record Actual Result, Pass/Fail/Blocked, date, tester, evidence (screenshot/log), and defect ID if applicable.

**Important:** Do not mark tests as passed until they have actually been executed. Avoid uploading real facial data or sensitive personal data to a public portfolio.
