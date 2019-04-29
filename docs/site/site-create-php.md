---
layout: default
title: Site Create PHP
parent: Site
nav_order: 4
---

## Easy Engine Site Create

### ee site create -–type=php
Runs the standard PHP Site installation.

```
# Create html site
$ ee site create example.com

# Create html site with ssl from letsencrypt
$ ee site create example.com --ssl=le

# Create html site with wildcard ssl
$ ee site create example.com --ssl=le --wildcard

# Create html site with self signed certificate
$ ee site create example.com --ssl=self
```

### Options

| Argument                      | Description                                               |
|:------------------------------|:----------------------------------------------------------|
| `<site-name>`                 | Name of website                                           |
| `--cache`	                    | Use redis cache for PHP                                   |
| `--admin-email=<admin-email>` | E-Mail of the administrator.                              |
| `--with-db`                   | Create database for php site.                             |
| `--local-db`                  | Create separate db container instead of using global db   |
| `--php=<php-version>`         | PHP version for site. Currently only supports PHP 5.6 and latest.|
| `--dbname=<dbname>`           | Set the database name.                                    |
| `--dbuser=<dbuser>`           | Set the database user.                                    |
| `--dbpass=<dbpass>`           | Set the database password.                               |
| `--dbhost=<dbhost>`           | Set the database host. Pass value only when remote dbhost is required. |
| `--with-local-redis`          | Enable cache with local redis container.                  |
| `--skip-check`                | If set, the database connection is not checked.           |
| `--skip-status-check`         | Skips site status check.                                  |
| `--ssl=<value>`               | Enables ssl on site.                                      |
| `--wildcard`                  | Gets wildcard SSL                                         |
| `--force`                     | Resets the remote database if it is not empty.            |

#### Option PHP Version
5.6
{: .label .label-green }

7.2
{: .label .label-green }

Latest
{: .label .label-green }