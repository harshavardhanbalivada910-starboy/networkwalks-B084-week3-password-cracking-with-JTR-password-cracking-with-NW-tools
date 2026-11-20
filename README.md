# NetworkWalks – PDF Password Cracking Lab

## Overview
This repository documents my hands-on practice with the **NetworkWalks PDF password-cracking exercise**. The screenshots show the workflow of extracting a PDF hash, testing it with the site's built-in wordlist, recovering passwords, and opening the protected PDFs to capture the lab flags.

> **Learning/lab use only:** Perform password-recovery testing only on PDFs you own or are explicitly authorized to assess. Do not use recovered credentials against accounts, files, or systems without permission.

## Tools and environment
- **NetworkWalks Academy** – PDF Hash Extractor, Hash Calculator, and Password Cracker pages
- **WPS Office** – opening the password-protected PDF files
- **Browser** – accessing the NetworkWalks lab
- **Wordlist** – the site's built-in list (100 passwords), as shown in the screenshots

## Workflow

1. **Extract the PDF hash**  
   Use the PDF Hash Extractor provided in the lab to obtain the hash for the authorized practice PDF.

2. **Prepare the hash**  
   Use the NetworkWalks Hash Calculator page as directed by the exercise, then copy the resulting PDF hash.

3. **Run the password test**  
   Paste the hash into the Password Cracker page. Select the built-in 100-password list (or an authorized `.txt` wordlist) and start the test.

4. **Review the result**  
   The progress screen shows attempted candidates and the number tested. In the supplied example, the tool reports a match after testing candidates.

5. **Open the protected PDF**  
   Use the recovered password to open the corresponding PDF in WPS Office and view the lab completion message/flag.

## Results shown in the screenshots

| Practice PDF | Recovered password | Evidence |
|---|---|---|
| Example PDF 1 | `password1` | [Password result](screenshots/02-password-cracked-password1.jpg) |
| Example PDF 2 | `1qaz2wsx` | [Password result](screenshots/03-password-cracked-1qaz2wsx.jpg) |

The first cracking-progress screenshot records **66 of 100** candidates tested at that moment. The later success screenshot shows a match for `password1`.

## Captured lab flags

The supplied WPS Office screenshots show these completion flags:

- **Persistence / John the Ripper exercise:** `nw[networkwalks_persistence_jtr_270521]`
- **First flag:** `nw[networkwalks_flag1_jtr_270521_1]`

These values are transcribed from the screenshots. Keep flags and recovered passwords within the authorized training environment.

## Screenshots

### Password-cracking progress
![Password-cracking progress](screenshots/01-cracking-progress-66-percent.jpg)

### Recovered password: `password1`
![Password cracked: password1](screenshots/02-password-cracked-password1.jpg)

### Recovered password: `1qaz2wsx`
![Password cracked: 1qaz2wsx](screenshots/03-password-cracked-1qaz2wsx.jpg)

### PDF completion flag – persistence exercise
![Persistence exercise flag](screenshots/04-persistence-flag.jpg)

### PDF completion flag – first flag
![First flag](screenshots/05-first-flag.jpg)

## Key takeaways
- A wordlist attack tests candidate passwords against a supplied hash.
- The result depends on whether the correct password is present in the selected wordlist.
- A successful hash match provides the password needed to open the protected practice PDF.
- This exercise demonstrates password-auditing concepts in a controlled training environment.

---
**Project type:** Cybersecurity / Ethical Hacking Lab  
**Topic:** PDF password recovery using a wordlist  
**Evidence:** Screenshots from the completed NetworkWalks practice exercise
