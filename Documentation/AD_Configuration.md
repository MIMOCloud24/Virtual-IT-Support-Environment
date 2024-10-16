# Active Directory Configuration

## 1. Installing Active Directory Domain Services (AD DS)
- After installing Windows Server, open the **Server Manager**.
- Go to **Manage > Add Roles and Features**.
- Select **Active Directory Domain Services (AD DS)** and complete the installation.

## 2. Promoting the Server to a Domain Controller
- Once AD DS is installed, promote the server to a Domain Controller.
- Set up the domain (e.g., `example.com`).

## 3. Creating Organizational Units (OUs)
- In the **Active Directory Users and Computers** tool, create new OUs to organize users and devices:
  - Example: `OUs for different departments like IT, HR, etc.`

## 4. Creating User Accounts
- Create user accounts within the appropriate OUs.
