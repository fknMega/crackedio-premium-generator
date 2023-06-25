
make a new tampermonkey script,
insert this:
```
// ==UserScript==
// @name         GitHub Button Clicker
// @namespace    your-namespace
// @version      1.0
// @description  Clicks a button on GitHub page
// @author       Your Name
// @match        https://github.com/fknMega/crackedio-premium-generator
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // Function to find and click the button
    function clickButton() {
        var button = document.querySelector('.js-toggler-target.rounded-left-2.btn-sm.btn.BtnGroup-item');
        if (button) {
            button.click();
        }
    }

    // Wait for the page to load
    window.addEventListener('load', function() {
        // Click the button
        clickButton();
    });
})();

```

(you must be logged to github.com)
and after press f5
