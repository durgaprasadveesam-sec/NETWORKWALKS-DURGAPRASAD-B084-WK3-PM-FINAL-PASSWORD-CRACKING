# Networkwalks Internship — Week 3 Project Modules
## Password Cracking with JTR and Networkwalks Tools

**Candidate:** Durgaprasad Veesam (Batch B084)

This repository documents the completion of Week 3 Essential Project Modules for the Networkwalks Cybersecurity Internship — password cracking using both John the Ripper (JTR/Johnny) and Networkwalks' own online tools.

---

## Module 1: Password Cracking with JTR (John the Ripper + Johnny GUI)

**Task:** Crack the password of `My Locked PDF1.pdf` using John the Ripper and the Johnny GUI on Windows.

1. Installed John the Ripper and configured Johnny GUI to use it.

![Setting Up John the Ripper and Johnny GUI](<1. Setting Up John the Ripper and Johnny GUI.png>)

2. Extracted the crackable hash from `My Locked PDF1.pdf` using an online PDF hash extractor.

![Extracting the PDF Hash](<2. Extracting the PDF Hash.png>)

3. Saved the extracted hash into a text file (`hash1.txt`).

![Saving the Hash into a Text File](<3. Saving the Hash into a Text File.png>)

4. Loaded the hash file into Johnny and started the cracking attack.

![Running the Password Cracking Attack](<4. Running the Password Cracking Attack.png>)

5. Password successfully cracked: **`good-luck`**

![Password Cracked Successfully](<5. Password Cracked Successfully.png>)

6. Opened `My Locked PDF1.pdf` with the cracked password and captured the flag:
`nw{cybersecurity_flag_captured_2608}`

![Opening the PDF with the Cracked Password](<6. Opening the PDF with the Cracked Password.png>)

---

## Module 2: Password Cracking with Networkwalks Tools

**Task:** Crack a locked PDF using Networkwalks' own browser-based Hash Calculator and Password Cracker tools.

7. Extracted the hash from the locked PDF using the Networkwalks Hash Calculator.

![Extracting Hash with Networkwalks Hash Calculator](<7. Extracting Hash with Networkwalks Hash Calculator.png>)

8. `My Locked PDF1.pdf`'s password wasn't in the built-in 100-word list, so (as guided by the instructor) switched to `My Locked PDF2.pdf`. Successfully cracked using the Networkwalks Password Cracker: **`password1`**

![Cracking the Password with Networkwalks Password Cracker](<8. Cracking the Password with Networkwalks Password Cracker.png>)

9. Verified by opening `My Locked PDF2.pdf` with the cracked password.

![Verifying the Cracked Password Opens PDF2](<9. Verifying the Cracked Password Opens PDF2.png>)

---

## Bonus: Cracking PDF3 with Both Methods

As an additional exercise covered in the live class, `My Locked PDF3.pdf` was cracked using both tools.

10. Cracked using John the Ripper / Johnny.

![Cracking PDF3 with John the Ripper](<10. Cracking PDF3 with John the Ripper.png>)

11. Cracked using the Networkwalks Password Cracker.

![Cracking PDF3 with Networkwalks Password Cracker](<11. Cracking PDF3 with Networkwalks Password Cracker.png>)

12. Verified by opening the PDF — flag captured: `nw{networkwalks_flag_260821_1}`

![Verifying the Cracked Password Opens PDF3](<12. Verifying the Cracked Password Opens PDF3.png>)

---

## Key Takeaways

- Password-protected files store their password as a **hash**, not the password itself — cracking tools recover the password by testing candidate words against that hash.
- Weak/common passwords (like `good-luck`, `password1`) can be cracked in seconds, while strong, random, lengthy passwords resist cracking for years — showing why password strength matters.
- The same cracking logic (hash extraction → dictionary attack) applies whether using a desktop tool like John the Ripper or a browser-based tool.

---
© Networkwalks Cybersecurity Internship — Batch B084
