# Local Storage
- Reference: https://diveinto.html5doctor.com/storage.html

> These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

* What we actually want

- Plenty of storage space
- Located on the client
- Lasts longer than a page refresh
- Lastly, doesn't get transmitted to the server

* This was possible before the creation of HTML5

# HTML5 Storage

- Local storage or DOM storage

> So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

- Well, the latest version of pretty much every browser supports HTML5 Storage.

### Javascript 

> From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.

- check for HTML5 Storage
- https://diveinto.html5doctor.com/detect.html#modernizr (HTML5 detection library)


# Using HTML5 Storage

- HTML5 Storage is based on named key/value pairs
- You store data based on a named key, then you can retrieve that data with the same key. 
- The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. 
- In order to store and retrieve anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

- Calling setItem() with a named key that already exists will silently overwrite the previous value. Calling getItem() with a non-existent key will return null rather than throw an exception.

- Like other JavaScript objects, you can treat the localStorage object as an associative array. Instead of using the getItem() and setItem() methods, you can simply use square brackets.

> Calling `setItem()` with a named key that already exists will silently overwrite the previous value. Calling `getItem()` with a non-existent key will return null rather than throw an exception.

### In order to clear to the entire storage area and remove the value of a given named key (delete all keys and values at one time)

- interface Storage
- deleter void removeItem (in DOMString key);
- void clear();

* calling the removeItem() method with a non existent key will do absolutely nothing

## Tracking changes to the HTML5 Storage Area

- To keep track of storage area changes programmatically, the storage event can be trapped.  
- In order to hook the storage event a browser check will need to be done in order to see what event mechanism the browser supports.

## HTML5

- 5 Megabytes is how much storage space each origin gets by default 

- “QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes

# Web SQL Database 

- Similar to backend database programming except it can be done through javascript 
