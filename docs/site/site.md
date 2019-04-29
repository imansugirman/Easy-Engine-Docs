---
layout: default
title: Site
nav_order: 4
has_children: true
permalink: docs/site
---

## Easy Engine Site

Performs site operations. Check ee help site for more info.

Invoked function of `site-type` routing. Called when ee site is invoked. Performs the routing to respective site-type passed using either `--type=`, Or discovers the type from the site-name and fetches the type from it, Or falls down to the default site-type defined by the user, Or finally the most basic site-type and the default included in this package, `type=html`.

### Subcommand

| List                                      | Description                                           |
|:------------------------------------------|:------------------------------------------------------|
| [ee site clean](/docs/site/site-clean)    | Clears Object and Page cache for site                 |
| [ee site html](/docs/site/site-create-html) | Runs site installation with provided site type.    |
| [ee site php](/docs/site/site-create-php)  | Runs site installation with provided site type.    |
| [ee site delete](/docs/site/site-delete)  | Deletes a website.                                    |
| [ee site disable](/docs/site/site-disable)| Disables a website. It will stop and remove the docker containers of the website if they are running |
| [ee site enable](/docs/site/site-enable)  | Enables a website. It will start the docker containers of the website if they are stopped |
| [ee site info](/docs/site/site-info)      | Display all the relevant site information, credentials and useful links |
| [ee site list](/docs/site/site-list)      | Lists the created websites.                       |
| [ee site reload](/docs/site/site-reload)  | Reload services in containers without restarting container(s) associated with site  |
| [ee site restart](/docs/site/site-restart)| Restarts containers associated with site.             |
| [ee site share](/docs/site/site-share)    | Suppress informational messages                    |
| [ee site ssl](/docs/site/site-ssl)        | Show all PHP errors; add verbosity to EE bootstrap.   |
| [ee site update](/docs/site/site-update)  | Show all PHP errors; add verbosity to EE bootstrap.   |
