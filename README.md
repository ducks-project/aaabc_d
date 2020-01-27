ANOTHER AWESOME AUTOLOAD BESIDE COMPOSER FOR DRUPAL
============

Provide a simple autoload with composer for Drupal 7.


INTRODUCTION
------------

There's a lot of autoloader module for Drupal in 7.x.
So why should you use this one?
Simply because it's simple!
You just should use composer normally like it was on Drupal 8.
No overkill module or hook because autoloading and register must be 
the composer job.
All this module do is to include the composer "autoload.php" at a key event. 
This is why the module is named like that. Because of the drupal core files inclusion priority. 
For example, if you want to *use* (in your .module) a class from another module without *include* the file and the module name is alphabetically after your one, then Drupal 7 will throw an error.
This module will fix that.

 * For a full description of the module, visit the project page:
   https://drupal.org/project/aaabc_d

 * To submit bug reports and feature suggestions, or to track changes:
   https://drupal.org/project/issues/aaabc_d


REQUIREMENTS
------------

This module currently use a Drupal >= 7.x.


INSTALLATION
------------

 * Download and Install [composer](https://getcomposer.org/doc/00-intro.md)
 * Download and Install aaabc_d module with composer. `composer require drupal/aaabc_d`
 * Enable aaabc_d module.

You can use composer to install and manage dependencies like it's done on [Drupal 8](https://www.drupal.org/docs/develop/using-composer/using-composer-to-install-drupal-and-manage-dependencies).


CONFIGURATION
-------------

No configuration needed.


TROUBLESHOOTING
---------------

 * Unknown. But keep in mind that you now use the composer `autoload.php` file. So, you also need to tell composer where you're files live in. Like in Drupal 8 "optimized-autoload" will not correctly seek files on your module website directory if it already exist in your contrib repository.

FAQ
---

Q: Is a baby panda is cute?

A: Of Course, but less than a baby firefox.

MAINTAINERS
-----------

Current maintainers:
 * Adrien Loyant (donaldinou) - https://www.drupal.org/u/donaldinou

