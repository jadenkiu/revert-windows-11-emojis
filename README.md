# revert-windows-11-emojis
<h1>Step-by-step guide on how to revert Windows 11's fluent emojis back to the Windows 10 emojis.</h2>

<h4>*DISCLAIMER: FOLLOW THIS GUIDE AT YOUR OWN DISCRETION, THIS GUIDE WILL NOT TAKE RESPONSIBILITY FOR ANY POTENTIALLY HARMFUL CONSEQUENCES*</h4>

<h3>Windows Registry Editor Warning:</h3>
<p>Warning: Exercise extreme caution when using the Registry Editor. If you edit the registry incorrectly, serious problems might occur that could require a complete reinstall of the operating system and result in data loss. Avoid any edits suggested by unofficial sources.  For added protection, before making edits based on officially published Microsoft documentation, be sure to back up the registry. Then you can restore it if a problem occurs. For more information see </p> [How to back up and restore the registry in Windows](https://support.microsoft.com/en-us/topic/how-to-back-up-and-restore-the-registry-in-windows-855140ad-e318-2a13-2829-d428a2ab0692)<p>.</p>

<h2>Part 1 - Reverting Font</h2>

<h4>Step 1:</h4>
<p>Download the Windows 10 emoji font [here](/content/seguiemj.ttf).</p>

<h4>Step 2:</h4>
<p>Open Windows Registry Editor: Press Windows Button + R, type "regedit" and hit enter.</p>

<h4>Step 3:</h4>
<p>Navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts
Press "S" and find "Segoe UI Emoji".</p>

<h4>Step 4:</h4>
<p>Right click "Segoe UI Emoji" and delete, press "yes" when warned.</p>

<h4>Step 5:</h4>
<p>Navigate to where you downloaded the Windows 10 emoji font, the file named should be [seguiemj.ttf](/content/seguiemj.ttf).
Right click "seguiemj.ttf" and click "Install"
![Install option from right click menu](/markup-files/Right%20click%20menu%20install.png)</p>

<h4>Step 6:</h4>
<p>Restart your computer.</p>