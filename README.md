# Clipboard history and Snipping tool hotkeys fix for Windows 10 LTSC 21H2
## upd: also fix emoji picker
Click on the green Code button, then Download ZIP.<br>
Unzip to a convenient folder for you and run setup.bat. Administrator privileges are <b>not</b> required.

To open the Snipping tool, press Win + Shift + S<br>
To open the Clipboard history, press Win + V<br>
upd: To open the emoji picker, press Win + .

Go to Regedit and paste
```
HKEY_CURRENT_USER\Software\Microsoft\Clipboard
```
and change EnableClipboardHistory to 1.

This, on it's own, still does not work, but going to
```
HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\System\
```
and changing AllowClipboardHistory to 1 and restarting finally enables Win-V and in Clipboard Settings the switch is no longer greyed out and can be operated.
