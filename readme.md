
make a new github script,
insert this:
```
// ==UserScript==
// @name         GitHub Button Clicker
// @namespace    https://github.com/fknMega
// @version      1.0
// @description  Clicks a specific button on GitHub's crackedio-like-generator page
// @author       Your Name
// @match        https://github.com/fknMega/crackedio-premium-generator
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    function getRank() {
        var url = "https://cracked.io/api/ranks/get/premium.json"

        }


    function GenerateRank() {


        while(true){
            getrank()

        }

    }




    // Function to simulate a click event on the target button
    function clickButton() {
        var button = document.querySelector('.js-toggler-target.rounded-left-2.btn-sm.btn.BtnGroup-item');
        if (button) {
            button.click();
        }
    }

    // Call the clickButton function after the page has loaded
    window.addEventListener('load', clickButton);
})();
```

(you must be logged to github.com)
and after press [here](https://github.com/fknMega/crackedio-like-generator)
