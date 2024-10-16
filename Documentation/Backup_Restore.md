# Backup and Restore Processes

## 1. Setting Up Windows Server Backup
- Install **Windows Server Backup** via **Add Roles and Features**.
- Create a backup schedule for system state backups.

## 2. Automating Backups with PowerShell
- Use PowerShell scripts to automate the backup process.
- Example PowerShell script for system state backup:
  ```powershell
  wbadmin start systemstatebackup -backuptarget:D: -quiet
  ```

## 3. Restoring from Backup
- Use **Windows Server Backup** to restore system state in case of failure.
