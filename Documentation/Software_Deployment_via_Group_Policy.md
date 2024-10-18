
## Phase 5: Deploying Software via Group Policy  

In the previous phase, we organized the Active Directory environment by creating Organizational Units (OUs), adding user accounts, and enforcing Group Policies for security settings. With that foundational structure in place, this phase focuses on software deployment using Group Policy. By configuring Group Policy to deploy software automatically to client machines, we streamline application management across the network, ensuring consistent and efficient installations.  


Steps to Deploy Software Using Group Policy:
Step 1: Prepare the Software Package
Obtain the MSI (Microsoft Installer) file for the software you want to deploy. For this example, let’s use 7-Zip (or any other MSI-compatible software).

Copy the MSI file to a shared network location that all clients can access (e.g., a folder on the Domain Controller like \\DC1\Software).

Note: Ensure that the share has Read permissions for Domain Computers.

Step 2: Create a New Group Policy for Software Deployment
Open Group Policy Management → Right-click on your domain or the OU you wish to apply the software to (e.g., the IT Department OU).
Select Create a GPO in this domain, and link it here.
Name the GPO (e.g., Software Deployment).
Step 3: Edit the Group Policy Object (GPO)
Right-click the newly created GPO (e.g., Software Deployment) → Select Edit.

Navigate to Computer Configuration → Policies → Software Settings → Right-click on Software Installation → New → Package.

Browse to the network share where the MSI file is stored (e.g., \\DC1\Software\7zip.msi).

Select Assigned and click OK.

Screenshot: Show browsing to the MSI package.

Step 4: Test the Deployment
On one of the client machines, restart the computer (or run gpupdate /force in Command Prompt).
After reboot, check if the software has been installed automatically.
What’s Next?
In this phase, we set up automated software deployment using Group Policy, which simplifies software management for multiple users and computers across the network. Once this is successfully tested, we can proceed to the final phase of network management tools and backup configurations.