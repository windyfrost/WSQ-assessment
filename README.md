# WordPress Webshell Plugin (Educational Use Only)

⚠️ **Disclaimer:**  
This plugin is intended **solely for educational and research purposes**. It demonstrates how vulnerable or misconfigured WordPress installations can be exploited through plugin uploads. **Do not use this on systems you do not own or have explicit permission to test.**

## 📘 Overview

This project provides a minimal, proof-of-concept WordPress plugin that, once installed and activated, can generate a reverse shell back to a listener of your choice. It is meant to support ethical hacking students learning about web exploitation and privilege escalation within CMS environments.

The plugin follows valid WordPress structures to avoid rejection during installation, and executes shell commands based on incoming parameters.

## 🔍 Features

- ✅ Valid WordPress plugin structure
- 🎯 Easy to deploy and activate
- 🌀 Reverse shell execution via attacker-controlled listener
- ⚙️ Lightweight and minimal footprint


## ⚙️ Usage

### 1. Setup Your Listener

Before uploading the plugin, start your listener using Netcat or any preferred tool:

```bash
nc -lvnp 4444
```

### 2. Modify the Plugin

Replace the IP and port in `webshell-plugin.php` with your listener's details.

### 3. Create ZIP and Upload

Compress the plugin folder and upload it to WordPress via:
`Plugins > Add New > Upload Plugin`

Then activate the plugin.

## 🛡️ Important Notes

- ❗ Only use this in lab or test environments.
- 🧹 Remove the plugin immediately after testing.
- 🔒 Never upload this to a live or production server.

## 👨‍🏫 For Students

This repository is part of an ethical hacking curriculum. Use it only in permitted CTFs or learning labs.

## 📜 License

This project is released under the **MIT License**. Use responsibly.
