Failed RDP to IP Geolocation Information

Description:

The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.

The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot. We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
Languages Used
PowerShell: Extract RDP failed logon logs from Windows Event Viewer

Utilities Used
ipgeolocation.io: IP Address to Geolocation API
Attacks coming in; Custom logs being output with geodata

<img width="650" alt="Screen Shot 1444-09-28 at 07 59 26" src="https://user-images.githubusercontent.com/126103226/232972909-6af02f92-08ff-4095-81bc-e88d7e701415.png">

World map of incoming attacks after 24 hours 
(built custom logs including geodata)<img width="747" alt="Screen Shot 1444-09-28 at 07 58 54" src="https://user-images.githubusercontent.com/126103226/232972976-1ad8efd0-5d73-4506-8a2c-6bec7a40a00a.png">
