---
Title: "File Scanning"
Slug: file-scanning
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 6800
---


## Enabled Scanners

At least one scanner must be enabled for vBulletin to scan uploaded files. <br />
Note that scanning is performed at the time of upload, and previously uploaded files will not be retroactively scanned after enabling a scanner.




- Variable Name: enabled_scanner
- Data Type: free
- Default Value: []

## Clamd Local Socket

Filepath to the unix socket used by the ClamAV Daemon (clamd). Alternatively (if using the TCP socket with clamd) you can use the "Clamd TCP Socket IP" & "Clamd TCP Socket Port" options.




- Variable Name: vbfilescan_clamd_sock
- Data Type: free
- Default Value: 

## Clamd Network Socket IP

IP Address for the network socket used by clamd. Leave this empty if using the "Clamd Local Socket" option. This is the "TCPAddr" value in the ClamAV Daemon's configuration (clamd.conf) file.




- Variable Name: vbfilescan_clamd_ip
- Data Type: free
- Default Value: 

## Clamd Network Socket Port

Port for the network socket used by the clamd. Only required if using the "Clamd Network Socket IP" option. This is the "TCPSocket" value in clamd.conf .




- Variable Name: vbfilescan_clamd_port
- Data Type: free
- Default Value: 


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>