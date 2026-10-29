# Requirement Traceability Matrix (RTM)

**Project:** Face Recognition System with KD-Tree  
**Status:** Draft mapping of designed tests; not proof of test execution

| Business requirement | Functional requirements | Designed test cases | Coverage note |
|---|---|---|---|
| BR-001: Support identification against registered data | FR-001, FR-002, FR-003, FR-004, FR-005 | Additional detection/matching test cases still needed | Partial |
| BR-002: Review unfamiliar face and decide whether to add it | FR-006, FR-007 | TC-001, TC-002, TC-003, TC-004, TC-006 | Designed tests cover review decision paths |
| BR-003: Manage registered face data | FR-009 | Exact scope and tests need confirmation | Pending |
| BR-004: Address privacy, access, errors, and human review | Proposed security/privacy NFRs | Additional requirements and tests needed | Pending |

## Notes
- “Designed tests cover” means test scenarios have been drafted, not that the system passed them.
- Add dedicated tests for known-face matching, unknown-face matching, face angle, lighting, appearance changes, and performance after checking the actual system and agreeing acceptance thresholds.
