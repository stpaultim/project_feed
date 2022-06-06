Project Feed
=====================

This module pulls down contrib project data from Github and creates nodes in a Backdrop CMS website. In theory, code checks for existing node and only creates new nodes when none exist. Ability to update nodes is coming soon?

This module is a result of the discussion started here:
https://github.com/backdrop-ops/backdropcms.org/issues/870

And this module is very much inspired by the sample conde snippet provided
by @BWPanda in that thread.

This modules is still very much in development. We welcome feedback and suggestions and Pull Requests.

This module is somewhat a proof a concept and sandbox for possible features on BackdropCMS.org and/or another third party module info site.

Coming Soon (ideas)
-------------

- Pulling in "tag" data from project .info file
- Pulling in additional data about Releases
- Pulling in additional download statistics
- Ability to update nodes

Requirements
------------

The Github API has [pretty strong limits](https://docs.github.com/en/rest/overview/resources-in-the-rest-api#rate-limit-http-headers) to how many requests you can make
per hour unless you are working with a [personal access token](https://docs.github.com/en/rest/overview/other-authentication-methods).


Installation
------------

-

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

- Keeping this in my personal repo for now. Feel free to post issues here.


Current Maintainers
-------------------

- [Tim Erickson](https://github.com/stpaultim).

Credits
-------

- Sponsored by [Simplo](https://www.simplo.site)
- Valuable code snippet provided by [@BWPanda](https://github.com/BWPanda)


License
-------

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.
