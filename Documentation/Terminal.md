# Windows Terminal

## 1. Install "Windows Terminal"

Using Chocolatey, simply run: "choco install microsoft-windows-terminal -y"

Using the Microsoft Store, search for "Windows Terminal" and download.

## 2. "Run as administrator" Fix

By default, Windows Terminal (Priview) runs as a UWP application, meaning it does not allow for elevation ("Run as Administrator").

To bypass this limitation, follow the steps below:

1. On your desktop, right-click and select "New", then "Shortcut".
2. In the new window that appears, enter "C:\Windows\System32\cmd.exe /c start /b wt", then click "Next".
3. Next, enter "Windows Terminal" to name the shortcut, then click "Finish".
4. Right-click the newly created shortcut, and select "Properties".
5. Download the "terminal.ico" icon and save it locally.
6. Back on the "Properties" window, select "Change Icon", and point it to the "terminal.ico" file you saved locally.
7. Back on the "Properties" window, select "Advanced", and check "Run as administrator", then click "OK".
8. Click "Apply" if available, "OK" if not.
9. (Optional) Drag the new shortcut to your taskbar and left-click it to open an elevated Windows Terminal session!

## 3. Cuztomise "Windows Terminal" Profile

Unlike PowerShell, the "Windows Terminal" profile is located in a file called "profiles.json".
It is located in: "$env:LocalAppData\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState"

For .gif files you would like to use as a background, you can add them to this path:
"$env:LocalAppData\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\RoamingState\"
