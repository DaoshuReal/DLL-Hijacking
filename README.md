# DLL-Hijacking

This project is a proof-of-concept demonstrating **DLL Hijacking** vulnerabilities in several popular Windows applications. Precompiled DLLs are provided to test and demonstrate how these applications may load malicious DLLs when placed in specific locations.

## 📌 What is DLL Hijacking?

**DLL Hijacking** is a technique where an attacker places a malicious DLL in a directory where a vulnerable application will load it instead of the legitimate one. This can result in the execution of arbitrary code within the context of the trusted application.

## 📁 Build Folder Structure

The `Build` folder contains subdirectories for various target applications:

``Build/
├── Brave/
├── Chrome/
├── Discord/
├── Epicgames/
├── Firefox/
└── Steam/``

Each subfolder contains a DLL named and structured to match a specific DLL expected by that application. Although the DLLs contain the same payload, they are renamed and intended to be used in different directory paths to trigger hijacking.

## 🛡 Disclaimer

This repository is intended for **educational and ethical testing** only. Do not deploy or test on systems you do not own or have explicit permission to audit.

> Misuse of this code may be illegal. Use responsibly and only in controlled environments.
