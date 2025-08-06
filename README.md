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
// @name         Aviago
// @namespace    https://badzone.co/
// @version      1.0.0
// @description  Modular, secure automation for Aviator game
// @author       BadZone
// @match        https://aviator-next.spribegaming.com/*
// @match        https://www.betpawa.rw/*
// @connect      firestore.googleapis.com
// @connect      pushover.net
// @require      https://cdn.jsdelivr.net/gh/Badzoneyv4n/aviago-dist@b717d7a/dist/aviago.secure.js
// @grant        GM_getValue
// @grant        GM_setValue
// @grant        GM_addValueChangeListener
// @grant        GM_xmlhttpRequest
// ==/UserScript==

(function() {
    'use strict';

    // Thank you for your time
})();
```
---
## 📌 Version Info

See `version.json` for current stable release.

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE) with additional disclaimers.