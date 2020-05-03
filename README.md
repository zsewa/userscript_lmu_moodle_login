# LMU Moodle Login Userscript
Stay logged in on LMU Moodle moodle.lmu.de

## Install
1) Install a userscript manager like [Tampermonkey](https://www.tampermonkey.net/) for your prefered browser.
2) Go to [Greasyfork](https://greasyfork.org/en/scripts/402556) and click on "Install this script"
3) The activated script will trigger on moodle.lmu.de

## How does it work?
This userscript is triggered on the LMU Moodle website.

It checks if you are logged in or not. 
If you are logged out, you are redirected to the LMU Login Provider (Shibboleth).
Occasionally Shibboleth should be able to restore the session without entering the user data. 
Otherwise you saved two clicks.
