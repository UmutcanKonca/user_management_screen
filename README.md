# User Management Screen Specification

## Overview

This document outlines the user interface specifications for the User Management screen. It provides detailed requirements, UI components, behaviors, and initial state details. This will guide software developers in implementing the user management functionality.

## Requirements

1. **User Listing**
    - Display a list of users with the following columns:
        - ID
        - User Name
        - Email
        - Enabled Status

2. **User Actions**
    - Add new users.
    - Edit existing users.
    - Toggle visibility of disabled users.

3. **User Form**
    - Form fields for creating or editing a user:
        - Username
        - Display Name
        - Phone
        - Email
        - User Roles (dropdown)
        - Enabled (checkbox)

## UI Components

### User List

- **Table Columns:**
    - **ID:** Numeric identifier for the user.
    - **User Name:** Username of the user.
    - **Email:** Email address of the user.
    - **Enabled:** Boolean status indicating if the user is enabled or disabled.

- **Buttons:**
    - **New User:** Opens the form to add a new user.
    - **Hide Disabled User:** Checkbox to toggle the visibility of disabled users in the list.

### User Form

- **Fields:**
    - **Username:** Input field for the username.
    - **Display Name:** Input field for the display name.
    - **Phone:** Input field for the phone number.
    - **Email:** Input field for the email address.
    - **User Roles:** Dropdown to select user roles (Guest, Admin, SuperAdmin).
    - **Enabled:** Checkbox to enable or disable the user.

- **Buttons:**
    - **Save User:** Saves the user information.

## Behavior

### Initial State

- On page load, the user list displays all enabled users.
- The "Hide Disabled User" checkbox is checked by default.

### User Interactions

- **New User Button:**
    - Opens a blank form on the right side for entering new user details.
    
- **Hide Disabled User Checkbox:**
    - When checked, hides users with `Enabled` status set to `false`.
    - When unchecked, displays all users.

- **User Form:**
    - **Save User Button:** Saves the new or edited user details and updates the user list.



