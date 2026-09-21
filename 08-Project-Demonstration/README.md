# Phase 8: Project Demonstration

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Demonstration Overview
This phase demonstrates the complete working of the Standard Laptop procurement automation developed using ServiceNow Flow Designer.

The demonstration covers the project objective, Flow Designer configuration, Standard Laptop request, approval process, automatic Catalog Task creation, and final output verification.

## Project Purpose
The purpose of this project is to automate the Standard Laptop procurement process and reduce manual intervention in IT operations.

After approval of a Standard Laptop request, the system automatically creates a Catalog Task and assigns it to the Hardware group.

## Demonstration Steps

### Step 1: Show the Flow Designer
Open the `Standard laptop task` flow in ServiceNow Flow Designer.

Demonstrate:
- Flow Name: Standard laptop task
- Application: Global
- Run As: System User
- Trigger: Service Catalog
- Action: Create Catalog Task

### Step 2: Show Catalog Task Configuration
Demonstrate the Create Catalog Task action with:

- Requested Item: Trigger → Requested Item Record
- Short Description: Laptop need to Configured
- Description: Laptop need to Configured
- Assignment Group: Hardware
- Approval: Approved

### Step 3: Show Standard Laptop Catalog Item
Open the Standard Laptop Catalog Item and demonstrate that the `Standard laptop task` flow is configured in the Process Engine.

### Step 4: Place Standard Laptop Order
Open the Service Catalog and select the Standard Laptop item.

Place the order using `Order Now`.

### Step 5: Show Request and Approval
Open the generated Request and demonstrate the approval process.

Approve the pending request.

### Step 6: Show Requested Item
Open the Requested Item generated for the Standard Laptop order and verify that the request has been approved.

### Step 7: Show Automatically Generated Catalog Task
Open the Catalog Tasks section and demonstrate the automatically generated task.

### Step 8: Verify Final Output
Verify the following details:

- Catalog Task: SCTASK0010001
- Requested Item: RITM0010001
- Short Description: Laptop need to Configured
- Description: Laptop need to Configured
- Assignment Group: Hardware
- Approval: Approved
- State: Open

## Final Workflow

Standard Laptop Request  
→ Request Created  
→ Approval  
→ Request Approved  
→ Flow Designer Automation  
→ Catalog Task Created  
→ Hardware Group Assigned  
→ Laptop Configuration

## Project Benefits

- Reduces manual intervention.
- Automates Catalog Task creation.
- Automatically assigns work to the Hardware team.
- Reduces delays in laptop configuration.
- Improves IT procurement efficiency.
- Provides a consistent procurement workflow.

## Demo Video

The complete project demonstration video will include:

- Project Name
- Purpose of the Project
- Benefits of the Project
- ServiceNow Flow Designer Configuration
- Project Execution and Working Process
- Approval Process
- Automatic Catalog Task Creation
- Final Output

## Project Demo Video

The complete project demonstration video includes the ServiceNow Flow Designer configuration, Standard Laptop procurement workflow, testing process, and final Catalog Task output.

**Demo Video:** [Watch Project Demonstration](https://drive.google.com/file/d/11zJNUuhb8p7EOGA4JLhh1RR5et6J97oW/view?usp=sharing)

## Final Result
The project was successfully implemented and tested using ServiceNow Flow Designer.

The Standard Laptop procurement process successfully generates a Catalog Task and assigns it to the Hardware group after approval.

## Project Status
Project Implementation and Demonstration Completed Successfully.
