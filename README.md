# revert-windows-11-emojis
## Step-by-step guide on how to revert Windows 11's fluent emojis back to the Windows 10 emojis.

#### *DISCLAIMER: FOLLOW THIS GUIDE AT YOUR OWN DISCRETION, THIS GUIDE WILL NOT TAKE RESPONSIBILITY FOR ANY POTENTIALLY DAMAGE TO YOUR OPERATING SYSTEM OR USER EXPERIENCE*
------------------------
### Windows Registry Editor Warning:
Warning: Exercise extreme caution when using the Registry Editor. If you edit the registry incorrectly, serious problems might occur that could require a complete reinstall of the operating system and result in data loss. Avoid any edits suggested by unofficial sources.  For added protection, before making edits based on officially published Microsoft documentation, be sure to back up the registry. Then you can restore it if a problem occurs. For more information see [How to back up and restore the registry in Windows](https://support.microsoft.com/en-us/topic/how-to-back-up-and-restore-the-registry-in-windows-855140ad-e318-2a13-2829-d428a2ab0692).

------------------------
Video guide coming soon
------------------------

### Part 1 - Reverting Font

#### Step 1:
Download the Windows 10 emoji font [here](/content/seguiemj.ttf).

#### Step 2:
Open Windows Registry Editor: Press Windows Button + R, type "regedit" and hit enter.

#### Step 3:
Navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts.
Press "S" and find "Segoe UI Emoji".

#### Step 4:
Right click "Segoe UI Emoji" and delete, press "yes" when warned.

#### Step 5:
Navigate to where you downloaded the Windows 10 emoji font, the file named should be [seguiemj.ttf](/content/seguiemj.ttf).
Right click "seguiemj.ttf" and click "Install"
![Install option from right click menu](/markdown-files/Right%20click%20menu%20install.png)

#### Step 6:
Restart your computer.

### Part 2 - Reverting icons on the Windows Emoji Keyboard:
![Windows 11 Fluent Emojis on emoji keyboard](/markdown-files/Windows%2011%20fluent%20emojis%20on%20emoji%20keyboard.png)


should turn into:


 ![Windows 10 Emojis on emoji keyboard](/markdown-files/Windows%2010%20emojis%20on%20emoji%20keyboard.png)

#### Step 1
Navigate to this file path in File Explorer:
```C:\Windows\WinSxS\amd64_microsoft-windows-font-truetype-segoeui_31bf3856ad364e35_10.0.22621.1_none_3251cf6d05fadea7```

#### Step 2
Take ownership of the folder AND the **existing** seguiemj.ttf file (just in case).
1. Right click the folder or the file.
2. Select "Properties" from the right click menu.
3. Go to the "Security" tab, then click the "Advanced" button.
4. Click the "Change" button (should be blue and clickable, may have the Administrator shield icon next to it).
5. Input your username into the big blank space in the pop up window, click "Check Name" when done.
6. Check the "Replace owner on sub containers objects" box.
7. Click "Apply", then "OK" on the Properties window.
8. Close and reopen the Properties window.
9. Go to the "Security" tab, then click the "Advanced" button.
10. Make sure you are on the "Permission" tab of the pop up window, click "Add".
11. Click on the blue "Select a Principal" text.
12. Check the "Replace all child object permission entries with inheritable permission entries from this object" box, then select Apply.
13. If this doesn't give you permission to move the files inside the folder, edit the permission and check "Full control" for your user.

#### Step 3
Copy and paste the seguimj.ttf (**that you downloaded**) into the "amd64_microsoft-windows-font-truetype-segoeui..." folder. Select the "Replace file in this destination" option, this might require your browser to be closed, so replace the file then restore this tab for instructions.

#### Step 4
Restart computer.

Guide created by [jadenkiu](https://github.com/jadenkiu).
Jaden Chung

Works Cited:
“Microsoft.” Microsoft Support, https://support.microsoft.com/en-us/windows/how-to-open-registry-editor-in-windows-10-deab38e6-91d6-e0aa-4b7c-8878d9e07b11. 