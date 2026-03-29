## PropertyProPlus Mobile QA Test Management

This repository contains the comprehensive QA documentation and test case suite for the PropertyProPlus Android Mobile Application. The documentation is derived from automated dumps and manual test records, focusing on mobile-specific workflows, offline synchronization, and field data collection.

## Project Overview

Project Name: PropertyProPlus Mobile
Application: Mobile Data Collector App
Test Environment:	Android, iOS, Windows
Test Objective: Ensure seamless field data synchronization, offline reliability, and accurate property valuation entry on mobile devices.
Test Type: Manual Functional, Offline/Sync, and Regression Testing.

## Documentation Structure

The testing repository is organized into several key data tracks:
Suites (Suites.csv): Categorizes tests into logical modules such as "Tenant Switch Functionality," "Login Logic," "Sync Back Workflows," and "Task-Specific Regression" (e.g., Task 391 associative array indexing).
Test Repository (Tests.csv): A detailed log of 280+ test cases, including:
Connectivity Tests: Behavior of the app under "WiFi/Data Off" vs "On" states.
Authentication: Multi-tenant switching, "Remember Me" logic, and secure login.
Sync Logic: Bi-directional synchronization between the Web portal and the Android app for Summary, Land, and Improvement tabs.
Summary (Summary.csv): High-level execution metrics indicating total test counts and suite distribution.

## Key Test Areas

1. Tenant & Authentication Management
Tenant Switching: Validating the "Change Company" modal and its error handling when offline.
Security: Testing password visibility toggles and credential persistence via the "Remember Me" checkbox.

2. Media & Documentation Handling
Uploads: Verifying the limit of 7-8 uploads and the ability to handle various file types (Images, PDF, Word).
In-Report Logic: Testing the "Include in Report" toggle to ensure field-collected media maps correctly to the final valuation document.
Camera Integration: Functional testing of the native camera capture within the app.

3. Synchronization & Offline Mode
Offline Data Entry: Capturing valuation data and photos without internet and ensuring they queue correctly for later sync.
Web-to-Mobile Sync: Ensuring changes made by an Admin on the web dashboard (e.g., Site Area, Market Value Range) reflect accurately in the app after a "Sync Back" action.
Conflict Resolution: Validating data integrity when a valuation is edited simultaneously on the web and mobile.

4. UI/UX & Field Validation
Input Controls: Testing specific UI elements like the "Yellow/Green" status indicators and scroll functionality in long lists.
Null Safety: Regression testing for document file paths to prevent app crashes (Null Pointer Exceptions).

## How to Execute Tests

Setup: Ensure the Android device has the latest build installed and access to the mnd or uat tenant environments.
Test Selection: Reference the TC_ID (e.g., Tc84cb417) to identify specific requirements and preconditions.
Reporting: Follow the structured steps in the Tests.csv file. Record actual results and update the Status (Pass/Fail) and Execution Date.
Issue Tracking: For any Fail status, include the "Actual Result" and relevant "Comments" to assist the development team in reproduction.

Prepared & Executed By: Asadullah Al-Galib
