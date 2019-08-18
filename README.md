# hunter

## first of all

install tampermonkey on your chrome.
```
http://tampermonkey.net/
```

## second
write down your init code like this.
```
// ==UserScript==
// @name         Hunter
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @match        https://www.zhipin.com/job_detail/?query=&city=101190400&industry=&position=
// @author       You
// @grant        none
// ==/UserScript==

(function() {
    'use strict';
    
    var panel = document.createElement('div');
    panel.id = 'app';
    document.body.append(panel);

  const script = document.createElement('script');
  script.charset = 'UTF-8';
  script.src = 'https://localhost/hunter/main.js';
  document.documentElement.appendChild(script);
    // Your code here...
})();
```

## build
run npm
```
npm run main
```

## press F5 of your chrome.
