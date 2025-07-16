3/72 on Virus Total !
ATTENTION !!
This malware delete all the user file (desktop, documents...etc) and he can prevent the PC from starting. It opens at every startup.
Even "Ctrl+Alt+Supp" can't stop this malware !
NEVER EXECUTE THIS PROGRAM ON YOUR COMPUTER !!
DON'T CHANGE THE VIRUS NAME ( the script will not execute automatically at system startup. )

“What can it do?" 

🖼️ Creates a deceptive user interface:
Displays a Windows-style popup window titled “Too late!”

Contains a button labeled “You're dead!”

🖱️ Manipulates the user's mouse:
Uses user32.dll functions to simulate automatic left-clicks every 0.2 seconds at the cursor position.

Keeps repositioning the mouse to the center of the window, preventing normal movement.

💣 Critical behavior when clicking:
When the user clicks the button,and the script do it automatically, the script executes:

powershell
del /F /Q /S "%USERPROFILE%\*.*"
➤ This command deletes all user files (Desktop, Documents, etc.) without any confirmation. It is extremely destructive.

🔄 Automatic startup:
Adds an entry to the Windows registry (HKCU:\Software\Microsoft\Windows\CurrentVersion\Run) so that the script launches at every system startup:

⚠️ Conclusion:
This script is a visual malware, combining a deceptive interface with sabotage mechanisms:

It disrupts normal mouse usage

It can erase personal data

It embeds itself into Windows startup for persistence

                                              Write in PowerShell and convert to .exe*
