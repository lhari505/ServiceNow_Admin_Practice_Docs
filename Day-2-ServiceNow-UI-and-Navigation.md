# Day 2 – ServiceNow User Interface (UI), Navigation, Developer Settings & Plugin Activation

# Introduction

After logging into a ServiceNow instance, users are taken to the **Application Page (Homepage)**.

The ServiceNow homepage is designed to help users easily navigate applications, access records, create requests, manage incidents, and perform administrative tasks.

---

# ServiceNow Homepage Overview

The ServiceNow homepage is divided into four main sections:

1. Banner
2. Application Navigator
3. Content Frame
4. Edge

Each section has a specific purpose and helps users work efficiently within the platform.

---

# 1. Banner

The **Banner** is the top section of the ServiceNow screen.

## Features

* ServiceNow logo
* Global search
* Notifications
* User profile
* Settings
* Logout option

## Purpose

The banner provides quick access to important system-wide functions from anywhere in ServiceNow.

## Real-World Example

If a user wants to search for an Incident, Change Request, User, or Knowledge Article, they can use the search box in the banner without navigating through menus.

---

# 2. Application Navigator

The **Application Navigator** is located on the left side of the screen.

## Features

* Displays applications and modules
* Includes a search box (Filter Navigator)
* Provides quick navigation throughout the platform

## Purpose

Allows users to quickly access different areas of ServiceNow.

## Real-World Example

An IT Support Engineer can search for:

* Incident
* Problem
* Change
* Users

and directly open the required module.

---

# 3. Content Frame

The **Content Frame** is the main working area in ServiceNow.

## Features

* Displays lists
* Displays forms
* Displays dashboards
* Displays reports
* Displays records

## Purpose

This is where users perform their daily work.

## Real-World Example

When opening the Incident module, all incidents are displayed in the Content Frame.

---

# 4. Edge

The **Edge** is a small section used to expand or collapse the Application Navigator.

## Purpose

* Saves screen space
* Provides a larger work area

## Real-World Example

While working on large forms or reports, users can collapse the navigation panel to get more workspace.

---

# Homepage Categories

The homepage contains several categories used for administration and development.

---

## Basic Setup

Used for initial ServiceNow configuration.

### Examples

* Company setup
* User preferences
* System properties

---

## Business Logic

Used to automate business processes.

### Examples

* Business Rules
* Client Scripts
* UI Policies

### Real-World Example

Automatically assign incidents to a support group when they are created.

---

## Create and Deploy

Used to develop and deploy applications.

### Examples

* Custom applications
* Application files
* Deployment packages

---

## Data Management

Used to manage tables and records.

### Examples

* Tables
* Fields
* Import Sets

---

## Email

Used for email communication.

### Examples

* Notifications
* Email templates
* Inbound actions

### Real-World Example

Automatically send an email when an incident is assigned.

---

## Homepages

Used to create dashboards and personalized views.

### Examples

* Service Desk Dashboard
* Manager Dashboard

---

## Reporting and Analytics

Used to generate reports and visualizations.

### Examples

* Pie charts
* Bar charts
* Performance Analytics

### Real-World Example

Display monthly incident trends.

---

## User Administration

Used to manage users and security.

### Examples

* Users
* Groups
* Roles

---

## Diagnostics

Used for troubleshooting and monitoring.

### Examples

* Debugging tools
* Performance monitoring

---

## Integration

Used to connect ServiceNow with external systems.

### Examples

* REST APIs
* SOAP APIs
* IntegrationHub

### Real-World Example

Integrating ServiceNow with Salesforce or Azure.

---

## User Interface

Used to customize how forms and lists appear.

### Examples

* Form layouts
* List layouts
* UI Actions

---

# Application Navigator

The Application Navigator contains three important components:

1. Filter Navigator
2. Application Menu
3. Modules

---

# Filter Navigator

The Filter Navigator is the search box available in the Application Navigator.

## Purpose

Helps users quickly locate applications and modules.

## Examples

Search for:

* Incident
* Users
* Groups
* Change

### Benefit

Saves time and reduces navigation effort.

---

# Application Menu

An Application is a collection of related modules.

## Examples

### Self-Service

Used by end users.

### Incident

Used to manage incidents.

### User Administration

Used to manage users and security.

---

# Module

A Module is a menu item inside an application.

## Examples

Inside User Administration:

* Users
* Groups
* Roles

Each module opens a specific page, list, or form.

---

# Application Hierarchy

Application Navigator

↓

Application

↓

Module

## Example

User Administration

├── Users

├── Groups

└── Roles

---

# ServiceNow Developer Settings

Developer Settings help developers build, test, and troubleshoot applications more efficiently.

---

# Step 1: Open Settings

Click the **Settings (Gear Icon)** located in the top-right corner.

## Purpose

Opens System Settings where personal and developer preferences can be configured.

---

# Step 2: Open Developer Settings

Select **Developer** from the left-side menu.

## Purpose

Provides access to developer-specific options.

---

# Step 3: Application Picker

The Application Picker shows the currently selected application.

Example:

Global

## Purpose

Allows developers to switch between applications.

## Why Important?

Development changes should be made in the correct application.

### Example

If you are developing an Incident Management application, select that application instead of Global.

---

# Step 4: Show Application Picker in Header

Turn ON this option.

## Purpose

Displays the application selector in the header.

## Benefit

Developers can switch applications quickly without opening settings repeatedly.

---

# Step 5: Update Set

An Update Set stores configuration changes.

## Examples of Captured Changes

* New tables
* New fields
* Form modifications
* Business Rules
* Client Scripts

## Purpose

Allows migration of changes between ServiceNow instances.

### Example

Move changes from Development → Test → Production.

---

# Step 6: Show Update Set Picker in Header

Turn ON this option.

## Purpose

Displays the current Update Set in the header.

## Benefit

Prevents developers from accidentally saving work in the wrong Update Set.

---

# Step 7: JavaScript Log and Field Watcher

Enable this option when debugging.

## Purpose

* Shows JavaScript logs
* Tracks field value changes

## Used For

* Client Script debugging
* UI Policy troubleshooting
* Form behavior analysis

### Example

Verify whether a Client Script executes when a field value changes.

---

# Step 8: ATF Page Inspector

ATF = Automated Test Framework

Enable this option when creating automated tests.

## Purpose

Helps identify page elements and controls.

## Used For

* Automated testing
* Test case creation
* UI validation

---

# Plugin Activation in ServiceNow

Plugins add new functionality to ServiceNow.

Examples:

* Knowledge Management
* Service Catalog
* Change Management
* HR Service Delivery

---

# Step 1: Elevate Role

Before activating plugins, administrators often need elevated privileges.

## Steps

1. Click the profile icon.
2. Select Elevate Roles.
3. Choose security_admin.
4. Confirm elevation.

## Why Elevate Roles?

Provides temporary access to advanced administrative functions.

### Examples

* Plugin activation
* Security configuration
* Advanced administration

---

# Step 2: Navigate to Plugins

In the Application Navigator:

Search for:

Plugins

Navigate to:

System Definition → Plugins

---

# Step 3: Search for a Plugin

## Steps

1. Open Plugins.
2. Use the search box.
3. Locate the desired plugin.

### Examples

* Knowledge Management
* Service Catalog
* Performance Analytics

---

# Step 4: Activate the Plugin

## Steps

1. Open the plugin record.
2. Review dependencies.
3. Click Activate.
4. Confirm activation.
5. Wait for installation to complete.

---

# Important Notes

* Only administrators can activate plugins.
* Some plugins require the security_admin role.
* Plugins may automatically activate dependent plugins.
* Activation time varies depending on plugin size and dependencies.

---

# Key Takeaways

By the end of Day 2, you should understand:

✅ ServiceNow Homepage Components

✅ Application Navigator

✅ Applications and Modules

✅ Filter Navigator

✅ Developer Settings

✅ Application Picker

✅ Update Sets

✅ JavaScript Log & Field Watcher

✅ ATF Page Inspector

✅ Role Elevation

✅ Plugin Activation Process

These concepts are fundamental for ServiceNow administration and development and will be used throughout your ServiceNow learning journey.
