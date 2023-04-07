# PowerShell-Privilege-Escalation

This PowerShell script demonstrates a technique known as "privilege escalation," which allows non-administrator users to run PowerShell commands with elevated privileges. The script checks whether the current user is a member of the local administrators group and, if so, runs a payload with administrative privileges. If the user is not a member of the group, the script sets an environment variable to execute a PowerShell script with elevated privileges and runs a system task to clean up disk space.

## Usage

1. Download the privilege-escalation.ps1 script from the repository.
2. Open PowerShell terminal as a normal user.
3. Navigate to the directory where the script is saved.
4. Execute the script by running the following command:

`.\UAC.ps1`

When you run the UAC.ps1 script, it will check whether the current user is a member of the local administrators group. If the user is a member, the script will execute a payload with administrative privileges. You can modify this payload to include any PowerShell commands you want to run with elevated privileges.

If the user is not a member of the local administrators group, the script will set an environment variable to execute a PowerShell script with elevated privileges and run a system task to clean up disk space. You can modify the PowerShell script to include any commands you want to run with elevated privileges.

## Security Implications

This script highlights the security implications of privilege escalation on Windows systems. Attackers can use techniques like this to gain administrative access to a system and carry out malicious activities, such as stealing data or installing malware. As a defender, it's important to understand how privilege escalation works and to implement appropriate security measures to prevent it.

## Contributions

Contributions are welcome! If you find any bugs or have suggestions for improving the script, please open an issue or submit a pull request.

## License

This script is released under the MIT License. See the LICENSE file for more details.
