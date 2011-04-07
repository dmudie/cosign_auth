-- SUMMARY --
I have taken the cosign module and created a "cosign_auth" module that works on Drupal 7.  This module is not dependent on the webserver_auth module and does not use or rely on the authmap table.

For a full description of the module, visit the project page:
  http://drupal.org/project/cosign_auth
To submit bug reports and feature suggestions, or to track changes:
  http://drupal.org/project/issues/cosign_auth

-- REQUIREMENTS --
  None.

-- INSTALLATION --
NOTE: this module was derived from the cosign.module. 

* you must be running your server within a cosign infrastructure.
	More info at: http://www.weblogin.org/
* download the cosign_auth module
* copy the module into your drupal modules directory
* enable the module through the ?q=admin/build/modules page
* configure the module through the ?q=admin/config/system/cosign_auth page
* add the logout block to your page with the ?q=admin/build/block page

The cosign_auth module is not dependent on any other contributed modules, it
does not use the webserver_auth module and does not use or rely on the authmap
table.

If is advisible that the user name used for Drupal UID=1 be a valid cosign
uniqname capable of authenticating with Cosign.  I have used phpmyadmin to
manually change the "name" in the "users" table to such a uniqname.  Of
course, with Drupal 7 you can know assign any user the same capabilities of
UID=1 (or so they claim!).

Current maintainers:
  Bob Riddle - http://www-personal.umich.edu/~bdr/
