# PDF Password Cracking with John the Ripper (JTR) on macOS

## Project Overview
This project demonstrates a hands-on password-cracking lab using **John the Ripper (JTR)** and its graphical interface **Johnny** on macOS. The lab focuses on extracting a PDF password hash, loading it into Johnny, running an authorized password-recovery attack, and viewing the recovered password.

## Tools Used
- **John the Ripper (JTR)**
- **Johnny** – graphical interface for John the Ripper
- **macOS (Apple Silicon)**
- **WPS Office / PDF file** – to view the protected PDF and lab result

## Lab Workflow
1. Install and launch John the Ripper / Johnny on macOS.
2. Prepare a hash file containing the PDF hash in the format supported by JTR.
3. Open Johnny and select **Open password file**.
4. Load the hash file.
5. Start a new attack and monitor the results.
6. View the recovered password in Johnny.
7. Verify the lab result by opening the PDF, where the exercise displays the completion flag.

## Screenshots & Results
### 1. Johnny Interface
Johnny was launched on macOS. The screenshot shows the application interface and an update compatibility notice.

### 2. Password Recovery Result
The lab screenshot shows Johnny successfully recovering the example PDF password:
- **Recovered password:** `good-luck`
- **Hash format displayed:** PDF / pdf-opencl

### 3. Lab Flag – Exercise 1
The lab PDF displays the completion message and flag:

`nw{cybersecurity_flag_captured_2608}`

### 4. Lab Flag – Exercise 2
The second lab PDF displays another completion message and flag:

`nw{networkwalks_persistence_jtr_270521}`

## What I Learned
- The purpose of password hashes and hash files in password-recovery exercises.
- How to use Johnny as a graphical interface for John the Ripper.
- How to load a hash file and run an authorized password-recovery attack.
- How to verify results in a controlled cybersecurity lab.
- The importance of using password-cracking tools only on files and systems I own or have explicit permission to test.

## Disclaimer
This project is for educational purposes and authorized cybersecurity practice only. Do not attempt to recover passwords from files or systems without permission.

---
**Lab:** Password Cracking with John the Ripper  
**Platform:** macOS  
**Status:** Successfully completed
