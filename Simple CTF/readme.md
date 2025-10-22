# TryHackMe Writeup: Simple CTF
<img width="542" height="181" alt="image" src="https://github.com/user-attachments/assets/f2d012a3-b974-45df-bf80-8d743c6f4dab" />

## Objective
Capture the user and root flags

## Reconnaissance
Began with a full TCP port scan
<img width="907" height="417" alt="Screenshot 2025-09-03 202745" src="https://github.com/user-attachments/assets/fabf93b5-6109-4a35-89a7-b4870b7f0f3e" />
Analyzing the above NMAP scan , we know the number of ports and their associated services running on the host. So there are 2 services running under port 1000 and ssh is running on the highest port.

## Enumeration
As port 21 was opened , tried to login by anonymous
<img width="911" height="656" alt="Screenshot 2025-09-03 203546" src="https://github.com/user-attachments/assets/d52a2d74-06b3-43dc-b01f-27a12dc6f4c7" />
