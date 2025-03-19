# Volatile Memory Forensics Exploring the critical role of analyzing system RAM in modern digital investigations.

## About the Project
Volatile memory forensics, also known as memory forensics, focuses on analyzing data stored in a computer’s RAM to uncover evidence of malicious activities.
## Why Volatile Memory Forensics?

- Volatile memory forensics is a vital part of cybersecurity and digital investigations:
- Detecting Elusive Threats: Many modern attacks, such as fileless malware, exist solely in memory, leaving no disk traces.

- Understanding System Behavior: Memory snapshots reveal active processes, network connections, and more, offering a glimpse of a system’s real-time state.

- Recovering Sensitive Data: RAM often contains encryption keys, credentials, and other data not saved to disk.

- Building Forensic Timelines: Analyzing memory helps reconstruct sequences of events, shedding light on the scope and impact of attacks.

## Files

- [malware.py](https://github.com/wayalbhushan/volatile-memory-analysis/blob/main/malware.py): Simulates a malware script that deletes itself after execution but remains in memory.
  
- [Malware_detect.py](https://github.com/wayalbhushan/volatile-memory-analysis/blob/main/Malware_Detect.py): Scans running processes for known malware names and flags suspicious activities.
## Steps to Simulate
Clone the Repository: Clone this repository to your local machine:
```bash
git clone https://github.com/wayalbhushan/volatile-memory-analysis
```
Run the Scripts Using PowerShell:
a. Open PowerShell and navigate to the project directory:
```
cd path\to\Volatile_Memory_Forensics
```
b. Execute the malware script:
```
python malware.py
```
This simulates malware by printing a message, deleting itself, and continuing to run in memory.

c. Run the detection script:
```
python Malware_Detect.py
```
The detection script will:

List all running processes on the system.

Search for processes with names matching known malware patterns.

Alert you if suspicious processes are detected.

Analyze the Results:

If malware processes are detected, the script will display their details (PID, name, command line, user).

You can take action to terminate malicious processes based on the findings.

Features
Real-time detection of malicious processes in memory.

Demonstrates the behavior of fileless malware that persists in RAM after file deletion.

Provides a practical example of using Python for digital forensics and cybersecurity.

Disclaimer
This project is for educational purposes only. It is designed to demonstrate concepts in volatile memory forensics and is not intended for malicious use.
