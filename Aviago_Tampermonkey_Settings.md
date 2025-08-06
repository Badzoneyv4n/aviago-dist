
## 🛠️ Tampermonkey Global Settings

### Security
- **Content Script API**: `UserScripts API`
- **Sandbox Mode**: `Force Raw`
- **CSP Headers**: `Remove entirely (possibly unsecure)`
- **Allow HTTP headers to be modified by scripts**: `Yes`
- **Default tab types to run scripts in**: `All tabs`
- **Allow scripts to access local files**: `Externals (@require and @resource)`
- **Allow scripts to access cookies**: `All but protected cookies (HttpOnly)`
- **Allow communication with cooperate pages**: `Tampermonkey + script version`
- **Subresource Integrity**: `Validate if possible`
- **@include Mode**: `Default`
- **Check @connect**: `Ask if unknown`
- **Store data in incognito mode**: `Temporary`
- **Page Filter Mode**: `Blacklist`
- **Whitelist Pages**:
  ```
  https:\/\/greasyfork\.org\/.*
  http://xkcd.com/970/
  ```
- **Blacklist Pages**:
  ```
  *example.org*
  *paypal.tld*
  *stripe.com*
  *https://deutsche-bank-24.tld*
  *https://bankofamerica.tld*
  /^.*(anssi.nonlocal.com\/\[\]render)\/([A|a]|\d|\+|=|\$)?$
  ```

### Downloads BETA
- **Download Mode**: `Default`
- **Whitelisted File Extensions**:
  ```
  /\.((txt|out|wut))$/
  /\.((txt|pdf|json|yaml|xml|csv))$/
  \.iso
  /\.((zip|tgz|tar|bin))$/
  /\.z[0-9]{2,2}$/
  .rss
  ```

### Userscripts
- **UserScript URL Detection**: `Auto`
- **Script Templates**:
  - ECMAScript 5
  - ECMAScript 6
  - CoffeeScript

### Experimental
- **Strict Mode**: `Default`
- **Top-Level Await**: `Default`

---

## ✅ Reminder
Tampermonkey allows exporting all of the above via the **Utilities Tab**, which bundles:
- Installed Userscripts
- Global settings
- Storage data



## 📜 Individual Script Settings (Per Script)

### General
- **Enabled**: ✅
- **Inject Mode**: `Auto`
- **Inject Into**: `Page`
- **Download URL**: Defined
- **Last Updated**: Custom (timestamped)
- **Position**: `Top`
- **Run At**: `document-start`

### Permissions
- **@grant**:
  - `GM_setValue`
  - `GM_getValue`
  - `GM_addValueChangeListener`
  - `GM_xmlhttpRequest`
  - `GM_registerMenuCommand`
  - `GM_unregisterMenuCommand`

### Resources & External Scripts
- **@require**: Loaded via jsDelivr (CDN)
- **@resource**: Custom scripts or config
- **@connect**: Enabled for backend (e.g., Firebase or FastAPI)

### Metadata & Versioning
- **@name**, **@namespace**, **@version**, **@author**
- **@description**: Defined per module (claimer, reloader, sync, etc.)
- **@match / @include / @exclude**: Site-specific
- **@license**: MIT or proprietary
- **@updateURL**, **@downloadURL**: Version-pinned (no @latest)

---

✅ Each script is modular, UUID-aware, listens to GM changes, and executes based on Firebase config or site detection.
