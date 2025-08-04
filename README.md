# Aviago Distribution
This repository contains the **compiled, bundled and obfuscated** version of the Aviago automation system.  
It is intended to be used **only through a trusted and approved distribution flow**.

> **Disclaimer**: This software is for personal use only. Any misuse is the user's responsibility.

---

## 🚀 How to Install Aviago in Tampermonkey
1. Make sure [Tampermonkey](https://www.tampermonkey.net/) is installed in your browser.
2. Click "Create a new script".
3. Replace everything with the snippet below 👇 (copy & paste to avoid errors) 
4. Save and close the editor.

```javascript
// ==UserScript==
// @name         Aviago 🛩️
// @namespace    https://badzone.co/aviago
// @version      1.0.0
// @description  Automation system for Aviator
// @author       Badzone
// @match        *://*/*
// @grant        GM_setValue
// @grant        GM_getValue
// @grant        GM_addValueChangeListener
// @grant        GM_xmlhttpRequest
// @require      https://cdn.jsdelivr.net/gh/Badzoneyv4n/aviago-dist@latest/dist/aviago.secure.js
// ==/UserScript==
```
---
## 📌 Version Info

See `version.json` for current stable release.

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE) with additional disclaimers.