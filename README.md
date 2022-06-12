Project Feed
=====================

This module will pull Backdrop CMS project data from Github into your local site.

Currently, it works in two steps:

1) You will fetch data from Github in 1 of 3 batches. The data is stored in a 
   CSV file on the server.
2) You will import data from CSV file using feeds.

This module is a result of the discussion started here:
https://github.com/backdrop-ops/backdropcms.org/issues/870

And this module is very much inspired by the sample conde snippet provided
by @BWPanda in that thread.

This modules is still very much in development. We welcome feedback and suggestions and Pull Requests.

This module is somewhat a proof a concept and sandbox for possible features on BackdropCMS.org 
and/or another third party module info site.

Coming Soon (ideas)
-------------

- Pulling in additional data about Releases
- Pulling in additional download statistics

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
3) Use one of these three triggers to download data from Github
     - admin/config/services/projects/settings/pull_projects_1
     - admin/config/services/projects/settings/pull_projects_2
     - admin/config/services/projects/settings/pull_projects_3
4) After each download, pull data into site with Feeds Importer "Backdrop Projects"
   Must list location for import of csv file as: `public://project-list.csv`


http://project-feed.lndo.site/admin/config/services/projects/settings/pull_projects_1

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
