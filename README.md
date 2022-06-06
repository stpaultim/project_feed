Project Feed
=====================

This module pulls down contrib project data from Github and creates nodes
in a Backdrop CMS website. 

This module is a result of the discussion started here:
https://github.com/backdrop-ops/backdropcms.org/issues/870

And this module is very much inspired by the sample conde snippet provided
by @BWPanda in that thread.

This modules is still very much in development. We welcome feedback and suggestions and Pull Requests.

This module is somewhat a proof a concept and sandbox for possible features on BackdropCMS.org and/or another third party module info site.

Coming Soon
-------------



Requirements
------------

The Github API has [pretty strong limits](https://docs.github.com/en/rest/overview/resources-in-the-rest-api#rate-limit-http-headers) to how many requests you can make
per hour unless you are working with a [personal access token](https://docs.github.com/en/rest/overview/other-authentication-methods).


Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://docs.backdropcms.org/documentation/extend-with-modules.

- Visit the configuration page under Administration > Configuration > Category >
  My Module (admin/config/category/my_module) and enter the required
  information.

- Additional steps go here...


Documentation
-------------

This is still in development, but it does work. 

Instructions:

1) Enable the module
2) Add Github User Name and Token here: admin/config/services/projects/settings
3) Put something in the range of 10-30 in "Queries Per Pull" (This is inaccurate and will be fixed soon)
4) Use this link to trigger a pull of projects: admin/config/services/projects/settings/pull_projects 


Issues
------

Bugs and Feature Requests should be reported in the Issue Queue:
https://github.com/backdrop-contrib/my_module/issues.


Current Maintainers
-------------------

- [Your Name](https://github.com/username)
- Seeking additional maintainers


Credits
-------

- Ported to Backdrop CMS by [Your Name](https://github.com/username).
- Originally written for Drupal by [Someone Else](https://github.com/username).
- Based on [Some Other project](https://github.com/example).
- Sponsored by [An Organization](https://example.org).


License
-------

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.
