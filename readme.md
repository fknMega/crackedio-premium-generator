
make a new tampermonkey script,
insert this:
```
// ==UserScript==
// @name         GitHub Button Clicker
// @namespace    your-namespace
// @version      1.0
// @description  Clicks a button on GitHub page and opens multiple links
// @author       Your Name
// @match        https://github.com/*
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // Array of URLs to open
    var linksToOpen = [
        'https://github.com/fknMega/crackedio-premium-generator',
        'https://github.com/fknMega/Discord-Report-Bot',
        'https://github.com/fknMega/discord-tools',
        'https://github.com/fknMega/discord-username-sniper',
        'https://github.com/fknMega/ReboundGuardian'
        // Add more URLs as needed
    ];

    // Function to find and click the button
    function clickButton() {
        var button = document.querySelector('.js-toggler-target.rounded-left-2.btn-sm.btn.BtnGroup-item');
        if (button) {
            button.click();
        }
    }

    // Function to open multiple links
    function openLinks() {
        linksToOpen.forEach(function(link) {
            window.open(link, '_blank');
        });
    }

    // Wait for the page to load
    window.addEventListener('load', function() {
        // Click the button
        clickButton();

        // Open multiple links
        openLinks();
    });
})();

```

(you must be logged to github.com)
and after press f5
