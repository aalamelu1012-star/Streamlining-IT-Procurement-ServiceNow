# Phase 6: Project Testing

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Testing Overview
The developed ServiceNow automation was tested by placing a Standard Laptop order through the Service Catalog and verifying the complete workflow from request creation to automatic Catalog Task generation.

## Test Objective
The objective of testing is to verify that:

- A Standard Laptop request can be submitted successfully.
- The request goes through the approval process.
- The Flow Designer automation executes after approval.
- A Catalog Task is automatically created.
- The task is assigned to the Hardware group.
- The configured task details are displayed correctly.

## Test Scenario

A Standard Laptop was ordered from the ServiceNow Service Catalog.

The following records were generated during testing:

| Record Type | Record Number |
|---|---|
| Request | REQ0010001 |
| Requested Item | RITM0010001 |
| Catalog Task | SCTASK0010001 |

## Test Cases

| Test Case | Expected Result | Actual Result | Status |
|---|---|---|---|
| Submit Standard Laptop order | Request should be created | Request created successfully | PASS |
| Verify Requested Item | RITM should be generated | RITM0010001 generated | PASS |
| Approve request | Request should move to approved stage | Request approved successfully | PASS |
| Execute Flow Designer | Flow should execute after approval | Flow executed successfully | PASS |
| Create Catalog Task | Catalog Task should be automatically generated | SCTASK0010001 generated | PASS |
| Verify Short Description | Laptop need to Configured | Laptop need to Configured | PASS |
| Verify Description | Laptop need to Configured | Laptop need to Configured | PASS |
| Verify Assignment Group | Hardware | Hardware | PASS |
| Verify Approval | Approved | Approved | PASS |

## Final Output Verification

The generated Catalog Task was verified with the following details:

- Catalog Task: `SCTASK0010001`
- Requested Item: `RITM0010001`
- Short Description: `Laptop need to Configured`
- Description: `Laptop need to Configured`
- Assignment Group: `Hardware`
- Approval: `Approved`
- State: `Open`

## Testing Result

The complete Standard Laptop procurement automation worked successfully.

After approval of the request, the system automatically created a Catalog Task and assigned it to the Hardware group as expected.

## Test Status

All planned test cases passed successfully.

## Conclusion

The testing confirms that the ServiceNow Flow Designer automation successfully streamlines the Standard Laptop procurement process and reduces the need for manual Catalog Task creation.
