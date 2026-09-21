# Active Directory & Client PC Setup Guide

![Windows Server](https://img.shields.io/badge/Windows%20Server-2025-0078D4?style=for-the-badge&logo=windows-server&logoColor=white)
![Windows 11](https://img.shields.io/badge/Windows%2011-Enterprise-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active%20Directory-AD%20DS-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)

A step-by-step lab guide for setting up an Active Directory Domain Controller (DC), creating users and Organizational Units (OUs), and joining/logging in from a Windows 11 client machine.

---

## 📌 Project Overview

This project demonstrates core Active Directory management tasks:
* Deploying a **Windows Server 2025** Domain Controller.
* Installing and configuring **Active Directory Domain Services (AD DS)**.
* Designing an **Organizational Unit (OU)** structure (`IT` and `Sales`).
* Provisioning user accounts with specific permissions.
* Authenticating a **Windows 11 Enterprise** client PC against the domain.

---

## 🚀 Step-by-Step Implementation

### Step 1: Set Up the Domain Controller (DC) & Client PC

1. Set up the lab environment with two virtual machines:
   * **Domain Controller:** Windows Server 2025 (handles authentication, authorization, logins, and password verification).
   * **Client Workstation:** Windows 11 Enterprise.

<img width="886" height="852" alt="Server Manager Overview" src="https://github.com/user-attachments/assets/920fd03a-41a3-4004-b155-9d96a0808cb7" />

---

### Step 2: Install Active Directory Domain Services

1. Open **Server Manager**.
2. Click **Manage** $\rightarrow$ **Add Roles and Features**.
3. Select **Active Directory Domain Services (AD DS)** from the server roles and complete the wizard.

<img width="894" height="580" alt="Add Roles and Features Wizard" src="https://github.com/user-attachments/assets/3e8b1e85-70b1-41c6-bbfb-a1a82344352d" />

4. To verify installed roles and management tools, navigate to the **Tools** tab in Server Manager.

<img width="342" height="233" alt="Server Manager Tools Menu" src="https://github.com/user-attachments/assets/6c9307a0-311c-4e55-88d4-1d37ffb94c9d" />

---

### Step 3: Configure OUs and Users

1. Open **Tools** $\rightarrow$ **Active Directory Users and Computers**.

<img width="622" height="186" alt="Active Directory Users and Computers Navigation" src="https://github.com/user-attachments/assets/dc14618b-aea3-4c05-9c8e-166087b9175d" />

2. Right-click your domain and create a main **Organizational Unit (OU)**.
3. Inside the main OU, create sub-OUs for departments (e.g., `IT` and `Sales`).

<img width="192" height="57" alt="Creating OUs" src="https://github.com/user-attachments/assets/9052be1b-c36e-4442-b648-959867848cb1" />  
<img width="439" height="331" alt="OU Structure" src="https://github.com/user-attachments/assets/5399f65f-b1bb-4723-9cb0-46b85524f924" />

4. Right-click the desired OU folder and select **New** $\rightarrow$ **User**. Fill in the user details, log-on name (User ID), and initial password.

<img width="450" height="388" alt="New User Creation Wizard" src="https://github.com/user-attachments/assets/fd9b76db-0ce5-4167-afb7-7c6777de1c8f" />

5. Once created, double-click the user to adjust properties, group memberships, and account settings as needed.

<img width="554" height="599" alt="User Account Properties" src="https://github.com/user-attachments/assets/39011ea4-cb24-4b04-9539-5e56517c9c62" />

---

### Step 4: Authenticate from the Client Workstation

1. Boot up the **Windows 11 Enterprise** client machine.
2. At the lock screen, select **Other user**.
3. Log in using the User Principal Name (UPN) format:

```text
user@[your_domain_name].local









