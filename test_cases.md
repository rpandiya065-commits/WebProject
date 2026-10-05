# Test Cases

| Test ID | Test | Expected Result |
|---|---|---|
| TC01 | Upload valid spreadsheet | File loads successfully |
| TC02 | Run transform with valid rows | Records are created/updated |
| TC03 | Verify Short Description | Source value appears in target |
| TC04 | Verify Description | Full description is imported |
| TC05 | Verify Caller | Caller reference resolves correctly |
| TC06 | Verify Priority | Correct priority is stored |
| TC07 | Verify State | Correct state is stored |
| TC08 | Re-import with Coalesce value | Existing matching record is updated instead of duplicated |
| TC09 | Check Transform History | Import result and errors are displayed |
| TC10 | Check invalid data | Invalid rows are rejected or reported for correction |
