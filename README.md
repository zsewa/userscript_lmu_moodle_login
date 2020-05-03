# LMU Moodle Login Userscript
Stay logged in on LMU Moodle `moodle.lmu.de`

## Install
1) Install a userscript manager like [Tampermonkey](https://www.tampermonkey.net/) for your prefered browser.
2) Go to [this scripts page on Greasyfork](https://greasyfork.org/en/scripts/402556) and click on "Install this script"
3) The activated script will trigger on `moodle.lmu.de`

## How does it work?
This userscript is triggered on the LMU Moodle website.

It checks if you are logged in or not. 
If you are logged out, you are redirected to the LMU Login Provider (Shibboleth).
Occasionally Shibboleth should be able to restore the session without entering the user data. 
Otherwise you saved two clicks.

## Security
Note that the accual log in is provided by the LRZ at the URL `lmuidp.lrz.de`.

You can easyly audit this scrip as it it very brief. 

The final redirect to the LRZ page is done by a `moodle.lmu.de` domain, this scripts works only on the moodle.lmu.de domain.

The script is triggered on two explicit URLs:
`https://moodle.lmu.de/`, the main page, and `https://moodle.lmu.de/user/policy.php` which you are redirected too by moodle if you are acessing a course while not authenticated.
This reduces the scripts ability to interact with actual courses.
