---
title: Local Account to Domain Account Transition Guide
date: 2023-11-08 23:05:39
tags: system administrator
---

To change from using a local account to a domain account (like the one provided with an email-like format), you need to join the computer to the domain represented by the "@jalarue.com" part of the account name. Here's a general process you'd follow, assuming you have the necessary permissions and network access to your company's domain controller.

<!-- more -->

## On a Windows 10 or Windows 11 Computer:

### 1. Back Up Data

Ensure that you back up any important data associated with the local account, as you'll be switching to a new user profile.

### 2. Connect to the Company's Network

Make sure your computer is connected to your company's network. This might require a VPN if you are doing this remotely.

### 3. Join the Domain

- Open the Settings app (you can press Win + I).
- Navigate to "System" and then "About".
- Find and click on "Access work or school" on the right pane.
- Click on "Connect" and then select "Join this device to a local Active Directory domain".
- Enter the domain name (jalarue.com) and when prompted, provide the username and password for a domain account that has permission to join computers to the domain (this might need to be done by your IT department).
- Follow the prompts to join the domain, which will include setting the domain account you'll use and possibly restarting the computer.

### 4. Log In with the Domain Account

- After the computer is part of the domain, you can log out of the local account.
- On the login screen, select "Other user".
- Enter the domain account credentials in the format `username@domain.com` or `DOMAIN\username` and log in. In your case, it would be `mohamed.ayoub.amara@jalarue.com` or `JALARUE\mohamed.ayoub.amara`.
- This will create a new user profile associated with the domain account.

### 5. Transfer Data

- After logging in with the domain account, you may want to transfer data from the local account to the new domain account profile. You can do this manually by copying files from the old profile directory to the new one.
- The path to user profiles is typically `C:\Users\`, so you might copy data from `C:\Users\mohamed.ayoub.amara` to `C:\Users\mohamed.ayoub.amara.jalarue`.

### 6. IT Department Involvement

- Typically, such operations are managed by the IT department. They may have specific procedures or scripts to migrate local profiles to domain profiles, transfer data, or set up new accounts with the necessary configurations and permissions.

**Please note that the exact steps can vary depending on the company's network infrastructure and policies. Always consult with your IT department before attempting to change account types, especially in a corporate environment.**
