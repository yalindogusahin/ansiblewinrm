# Ansible WinRM Port Opening Script

This repository contains a PowerShell script that helps in opening the WinRM port on Windows servers, enabling Ansible to establish a connection.

## Prerequisites

- Windows Server 2012 or later
- Administrator privileges on the target server
- PowerShell 3.0 or later

## Usage

1. Clone this repository to your local machine or download the PowerShell script directly.
2. Open a PowerShell session with administrator privileges.
3. Navigate to the directory where the script is located.
4. Run the following command to execute the script:

```powershell
.\Windows_winrm.ps1

5. The script will prompt you to confirm whether you want to enable WinRM. Type 'Y' and press Enter to proceed.
6. The script will make the necessary changes to open the WinRM port and configure the firewall rules.
7. After the script finishes running, you should be able to connect to the target server using Ansible over WinRM.


## Note
This script modifies the firewall settings to allow inbound connections on the default WinRM port (5986). Make sure you understand the security implications of opening this port before running the script in a production environment.
If you want to use a different WinRM port, you can modify the script accordingly before running it.
