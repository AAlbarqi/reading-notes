# THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

- userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.
- In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” 
- In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers.

#### HTML5 STORAGE
it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies.

##### HTML5 STORAGE SUPPORT
IE	FIREFOX	SAFARI	CHROME	OPERA	IPHONE	ANDROID
8.0+	3.5+	4.0+	4.0+	10.5+	2.0+	2.0+

check for HTML5 Storage

`function supports_html5_storage() {`
    `try {`
        `return 'localStorage' in window && window['localStorage'] !== null;`
        `} catch (e) {`
            `return false;}}`

#### USING HTML5 STORAGE
- Calling `setItem()` with a named key that already exists will silently overwrite the previous value. 
- Calling `getItem()` with a non-existent key will return null rather than throw an exception.
- Calling `removeItem()` with a non-existent key will do nothing.

#### STORAGEEVENT OBJECT
| PROPERTY |	TYPE |	DESCRIPTION |
| ------------- | ------------- | ------------- |
| key |	string |	the named key that was added, removed, or modified |
| oldValue | any | the previous value (now overwritten), or null if a new item was added |
| newValue | any | the new value, or null if an item was removed|
| url* | string | the page which called a method that triggered this change |