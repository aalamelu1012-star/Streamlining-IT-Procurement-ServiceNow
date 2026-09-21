# Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Project Overview

This project focuses on automating the standard laptop procurement process using ServiceNow Flow Designer. The automation reduces manual intervention and ensures that a catalog task is automatically created and assigned to the Hardware team after the Standard Laptop request is approved.

## Problem Statement

The existing IT procurement process involves manual activities that may cause delays in configuring standard laptops. This project automates the process to improve efficiency, reduce manual overhead, and ensure timely laptop configuration.

## Project Objective

- Automate the Standard Laptop procurement workflow.
- Reduce manual intervention in the procurement process.
- Automatically create a Catalog Task after approval.
- Assign the generated task to the Hardware group.
- Improve efficiency and reduce user waiting time.

## Technology Used

- ServiceNow
- ServiceNow Flow Designer
- Service Catalog
- Catalog Tasks
- GitHub

## Project Workflow

1. User places a Standard Laptop request through the Service Catalog.
2. The request is submitted for approval.
3. The request is approved.
4. ServiceNow Flow Designer triggers the automation.
5. A Catalog Task is automatically created.
6. The Catalog Task is assigned to the Hardware group.
7. The Hardware team can proceed with laptop configuration.

## Flow Configuration

**Flow Name:** Standard laptop task

**Application:** Global

**Run As:** System User

**Trigger:** Service Catalog

**Action:** Create Catalog Task

**Short Description:** Laptop need to Configured

**Description:** Laptop need to Configured

**Assignment Group:** Hardware

**Approval:** Approved

## Project Phases

1. Brainstorming & Ideation Phase
2. Requirement Analysis Phase
3. Project Design Phase
4. Project Planning Phase
5. Project Development Phase
6. Project Testing Phase
7. Project Documentation Phase
8. Project Demonstration Phase

## Final Result

The ServiceNow Flow Designer automation was successfully implemented and tested. After approval of a Standard Laptop request, a Catalog Task is automatically generated with the required description and assigned to the Hardware group.

## Conclusion

This project demonstrates how ServiceNow Flow Designer can streamline IT procurement by automating repetitive tasks. The solution reduces manual effort, improves task allocation, and provides a more efficient Standard Laptop procurement process.
