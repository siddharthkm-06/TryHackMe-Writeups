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

As Anonymous login was allowed, I got access and found ForMitch.txt file
<img width="1372" height="70" alt="Screenshot 2025-09-03 204540" src="https://github.com/user-attachments/assets/111ecfa9-0586-4f40-b8b0-19e6cbccb455" />

Even though this file did not have anything important but it says the passwords are weak and most likely available on wordlists.

As we noticed earlier that a webserver is running on port 80, we try to access it by opening it in a browser

<img width="1878" height="758" alt="Screenshot 2025-10-22 184555" src="https://github.com/user-attachments/assets/71666423-1f31-4f9d-bbff-db604c728bca" />

It was just a live default Apache live page, so to get more information we use Gobuster tool. Gobuster is a tool used for directory and file brute-forcing on web servers. It helps in discovering hidden paths and files by making numerous HTTP requests to identify resources that may not be publicly listed.
<img width="1382" height="186" alt="Screenshot 2025-09-03 204528" src="https://github.com/user-attachments/assets/2f3c39a0-d6d1-48f4-a43b-1647c26995e8" />

We got this directory /simple with 301 so let's access it on the browser
<img width="1919" height="762" alt="Screenshot 2025-09-03 204346" src="https://github.com/user-attachments/assets/814927f1-30f2-4331-b827-eec462b1c4c3" />



