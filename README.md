# Ransomware Simulation & C2 Infrastructure

> **⚠️ DISCLAIMER: EDUCATIONAL PURPOSE ONLY**
> This project was developed strictly for academic and educational purposes to understand the mechanics of malware, Command & Control (C2) architectures, and cryptographic operations. The author does not condone the use of this code for malicious activities. **Do not execute this software on systems you do not own or have explicit permission to test.**

## Overview

This project simulates a full ransomware attack chain, from the initial infection vector to file encryption and key management. It was designed to demonstrate how modern ransomware operates, communicates with a Command & Control (C2) server, and handles cryptographic keys securely.

The goal of this research is to improve detection mechanisms and incident response strategies by reverse-engineering the offensive workflow.

## Key Features

* **Client-Server Architecture:**
    * **Agent (Malware):** Deployed on the target machine, responsible for file discovery and encryption.
    * **C2 Server:** Centralized server for key management, agent tracking, and command issuance.
* **Cryptographic Implementation:**
    * Hybrid encryption scheme (Simulated or actual AES/RSA implementation).
    * Secure key exchange protocol between the agent and the server.
* **Secure Communication:**
    * Encrypted channel for C2 traffic to evade basic network sniffing.
* **Remote Control CLI:**
    * Administrator interface to interact with infected agents (e.g., list victims, send decryption keys, trigger commands).
* **Full Attack Lifecycle:**
    * Infection $\rightarrow$ Key Generation $\rightarrow$ Encryption $\rightarrow$ Decryption/Recovery.
