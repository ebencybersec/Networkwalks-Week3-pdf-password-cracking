# Week 3 - PDF Password Cracking

## Overview

As part of Week 3 of the Cybersecurity program at Networkwalks (Batch B082), I practiced password recovery against password-protected PDF files using three different approaches.

The activities were divided into three parts:

1. John the Ripper (JTR) and Johnny GUI on Windows
2. Networkwalks Hash Calculator and Password Cracker
3. John the Ripper with AI assistance using Hexstrike-AI MCP and Claude Desktop on Kali Linux

These exercises helped me understand how password-protected PDF files can be converted into crackable hashes and how password-cracking tools can be used in an authorized laboratory environment.

> **Ethical Use:** These techniques were performed only against provided lab files for educational purposes. Password-cracking tools should only be used against files or systems that you own or have explicit authorization to test.

---

# Part 1 - John the Ripper and Johnny on Windows

## Objective

The objective of this exercise was to recover the password of the provided `My Locked PDF1.pdf` file using John the Ripper and the Johnny graphical interface on Windows.

---

## Tools Used

- John the Ripper (JTR)
- Johnny GUI
- Windows PC
- PDF password hash

---

## Step 1 - Install John the Ripper

I downloaded John the Ripper from the official Openwall website and extracted/installed it on the Windows computer.

Official website:

https://www.openwall.com/john/

The `john.exe` executable is located inside the `run` directory of the John the Ripper installation.

### Screenshot

![John the Ripper Installation](screenshots/part1-john-installation.png)

---

## Step 2 - Install Johnny

I installed the Johnny graphical interface for John the Ripper.

Official information:

https://openwall.info/wiki/john/johnny

After installation, I opened Johnny and configured it to use the `john.exe` executable from the John the Ripper `run` directory.

### Screenshot

![Johnny Installation](screenshots/part1-johnny-installation.png)

---

## Step 3 - Extract the PDF Hash

The encrypted PDF file was processed using a PDF hash extraction tool.

The resulting hash started with:

```text
$pdf$
```

I copied the complete hash and saved it in a text file named:

```text
hash1.txt
```

The hash was saved without additional characters before $pdf$.

### Screenshot
### Screenshot

---

## Step 4 - Load the Hash into Johnny

I opened Johnny and loaded the `hash1.txt` file containing the PDF hash.

### Screenshot

---

## Step 5 - Start the Password Attack

I started a new password-cracking attack using John the Ripper.

### Screensho

---

## Step 6 - Verify the Password

After obtaining the password, I opened the encrypted PDF and entered the recovered password.

The PDF opened successfully, confirming that the password had been recovered.

### Screenshot

### Screenshot

---

# Part 2 - Networkwalks Hash Calculator and Password Cracker

## Objective

The objective of this exercise was to recover the password of the provided PDF using the Networkwalks Hash Calculator and Password Cracker through a web browser.

---

## Tools Used
- Networkwalks Hash Calculator
- Networkwalks Password Cracker
- Web browser
- Kali Linux or Windows

  ---
  
## Step 1 - Obtain the Lab PDF

I used the same `My Locked PDF1.pdf` file that I downloaded earlier from the Networkwalks lab page.

Lab page:

https://networkwalks.com/project-task-lab-password-cracking-with-networkwalks-tools/

### Screenshot

---

## Step 2 - Generate the PDF Hash

I opened the Networkwalks Hash Calculator:

https://networkwalks.com/hash-calculator/

I uploaded the encrypted PDF file.

The tool generated a PDF password hash beginning with:

```text
$pdf$
```
### Screenshot

### Screenshot

---


