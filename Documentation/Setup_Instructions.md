## Phase 1: Virtual Environment Setup

### Step 1: Install VMware Workstation Pro
1. Visit the [VMware's website](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion). 
2. Download and install VMware Workstation Pro. You will be asked to create an account. Once you do, download VMware WorkStation Pro.
3. When installing choose "for personal use" option to get free license.

![VMware Download Page](../Images/Screenshots/Vmware_Download_Page.png)
![VMware](../Images/Screenshots/Vmware_Installed.png)

4. It would be a good idea to organize vm's and virtual drives on separate folders.

![VM's and Virtual Drives folders(The path where they would be installed](../Images/Screenshots/VM's_&_Harddrives_folders.png)

## Step 2: Creating the windows server Virtual Machine 

1. Download ISO file of windows server 2022 and windows 10 or 11 from [Microsoft's Website](https://www.microsoft.com/en-us/evalcenter)

![Microsoft Evaluation center download page](../Images/Screenshots/Microsoft_Evalcenter.png)

2. You can use below Microsoft Generic keys to activate the windows.

![Microsoft windows Server Generic Keys](../Images/Screenshots/Windows_server_generic_keys.png)
![Microsoft windows 10 & 11 Generic Keys](../Images/Screenshots/Windows_10_&_11_generic_keys.png)

3. Open **VMware Workstation** and click **Create a New Virtual Machine**.
4. Select **Custom (Advanced)** for the configuration type. Click next twice.
5. Browse to the path where you save the windows server ISO file downloaded and click next.

![Browse Server ISO File](../Images/Screenshots/Browse_ISO_File_server.png)

6. input the Windows Product Key, choose the version of Windows Server to Install. "versions with core don't have GUI, but just command line. I will do this same project later with windows core version only." Click next.

![Product key window](../Images/Screenshots/Product_Key_Window.png)

7. Name your Windows Server VM and choose a directory path and click next.

![Vm Name](../Images/Screenshots/VM-Name.png)

8- Check UEFI and Secure Boot and then click next.<br>
9- chose how many processors and cores you want to assign your VM. (depends of what kind of processor you are running). Click Next.<br>
10- Specify how much RAM you want for your VM. Click Next.<br>
11- choose which network connection you want. I chose NAT so the VMs share the host machine’s IP address to access external networks. Click Next 3 times.<br>
12- Create new virtual disk. click Next.<br>
13- Specify your VM disk capacity. Click Next.<br>
14- choose a path where you want your virtual disk stored. Click Next.<br>
15- If you want to change anything or add/remove hardware, click Customize Hardware, otherwise click finish. 


![Vm Hardware Configuration](../Images/Screenshots/Vm_hardware_Configuration.png)

### Step 2. Installing Windows Server

After setting up the VM from first step, The VM will boot to Microsoft windows installation Page.

![Windows Installation screen](../Images/Screenshots/Windows_Installation.png)

1- Follow through the process. The ISO file I am using has 4 versions of Windows server 2022, I am choosing the standard version with Desktop experience.

![OS selection](../Images/Screenshots/OS-Version.png)

2- Follow through the steps.

![Installation Process](../Images/Screenshots/Windows_Installing.png)

3- Once done, The system will reboot, and asks you to set admin password. Type in your Strong Password and click Finish.

![Setting Admin Password](../Images/Screenshots/Setting_Admin_Password.png)

4- The system will apply settings, and get you to Log on Screen. Type in Your password and log in.

![Windows Server Logon](../Images/Screenshots/Windows_Log_ON.png)

5- Windows server will load, and opens up on Server Manager Automatically. That will conclude our Windows Server Installation.

![Windows Server ](../Images/Screenshots/Windows_Server.png)


### Step 3: Installing Windows Clients

Process of installing Windows Client is similar to Installing Windows Server.

1- Create VM for Windows 10 or Windows 11 client. Same as we did on Windows Server.

![VM Disk Creation](../Images/Screenshots/VM_Disk_Creation.png)

2- Install Windows 10

![Windows 10 Installation](../Images/Screenshots/Windows_10_Installation.png)

3- Follow through the steps. I am installing Windows 10 Pro.


![Windows 10 Pro Installation](../Images/Screenshots/Windows_10_Pro_Install.png)
![Windows 10 Pro Setup](../Images/Screenshots/Windows_10_Setup.png)

4- You will be asked to log in using Microsoft Account, I choose a local account.<br>
5- Follow the steps, choose a computer name, set up password. The windows will apply settings and load up.

This concludes our Windows 10 Client Installation on VMware VM.


![Windows 10 Pro Desktop](../Images/Screenshots/Windows_10_Desktop.png)


### Next Steps

With the virtual environment now set up and the operating systems installed on your VMs, the next phase of the project is to configure Windows Server as a Domain Controller by installing and setting up Active Directory Domain Services (AD DS). In this phase, you’ll create a domain, manage users and organizational units (OUs), and begin configuring Group Policies to manage and secure your network. Ensure that your VMs are fully operational before proceeding to this critical step.

















