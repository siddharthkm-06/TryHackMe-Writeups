# TryHackMe Writeup: The Game
<img width="628" height="168" alt="image" src="https://github.com/user-attachments/assets/057fb38e-6c99-4049-bbb0-86e6fb156a9c" />


## Objective
Find the hidden flag in the provided file.

## Tools Used
- Sysinternals `strings.exe` (Windows)

##  Extracting flag from the given file
To extract the flag from the executable, I used the following command:
`strings Tetrix.exe | findstr "THM{".`

![Screenshot 2025-09-03 162114](https://github.com/user-attachments/assets/d550e987-4169-4c39-928c-439ebfe26987)

The screenshot above shows the command output, confirming the hidden flag.

