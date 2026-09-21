# Phase 4: Project Planning

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Project Planning Overview
The project is planned to automate the Standard Laptop procurement process using ServiceNow Flow Designer.

The implementation is divided into multiple activities including requirement analysis, flow creation, catalog task configuration, flow assignment, testing, documentation, and demonstration.

## Project Goals
- Automate the Standard Laptop procurement process.
- Reduce manual intervention.
- Automatically create a Catalog Task after approval.
- Assign the generated task to the Hardware group.
- Test and verify the complete automation process.
- Document the implementation and final output.

## Project Tasks

| Task | Description |
|---|---|
| Requirement Analysis | Identify project requirements and expected output |
| Flow Creation | Create a new flow using ServiceNow Flow Designer |
| Trigger Configuration | Configure the Service Catalog trigger |
| Action Configuration | Configure the Create Catalog Task action |
| Flow Assignment | Assign the flow to the Standard Laptop catalog item |
| Request Testing | Place a Standard Laptop order |
| Approval Testing | Approve the generated request |
| Output Verification | Verify the automatically generated Catalog Task |
| Documentation | Document all project phases |
| Demonstration | Record the final working project |

## Implementation Plan

### Step 1: Analyze Requirements
Understand the project problem statement, objectives, user story, and expected output.

### Step 2: Create the Flow
Create a flow named `Standard laptop task` in ServiceNow Flow Designer.

### Step 3: Configure Trigger
Configure the flow with the `Service Catalog` trigger.

### Step 4: Configure Action
Add the `Create Catalog Task` action and configure the required task fields.

### Step 5: Assign the Flow
Assign the created flow to the `Standard Laptop` catalog item through the Process Engine.

### Step 6: Test the Request
Place an order for a Standard Laptop through the Service Catalog.

### Step 7: Approve the Request
Open the generated request and approve the pending approval.

### Step 8: Verify Automation
Verify that a Catalog Task is automatically created and assigned to the Hardware group.

### Step 9: Documentation
Prepare phase-wise documentation and upload the project files to GitHub.

### Step 10: Project Demonstration
Record a demonstration of the complete project workflow and final output.

## Resources Required
- ServiceNow Instance
- ServiceNow Flow Designer
- Service Catalog
- Standard Laptop Catalog Item
- Web Browser
- GitHub

## Risk and Mitigation

| Risk | Mitigation |
|---|---|
| Incorrect Flow Configuration | Verify trigger and action settings before activation |
| Flow Not Triggering | Verify the Process Engine configuration |
| Task Not Created | Check Flow Designer execution and Requested Item mapping |
| Wrong Assignment Group | Verify that the Assignment Group is set to Hardware |
| Approval Pending | Complete the request approval before verifying the task |

## Expected Result
The planned implementation should result in an automated Standard Laptop procurement process where an approved request automatically generates a Catalog Task assigned to the Hardware group.

## Project Status
Planning Completed.
