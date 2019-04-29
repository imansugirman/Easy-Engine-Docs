---
layout: default
title: Site Create Wordpress
parent: Site
nav_order: 5
---

## Easy Engine Create Wordpress

### ee site create --type=wp
Runs the standard WordPress Site installation.

```
# Create WordPress site
ee site create example.com --type=wp

# Create WordPress multisite subdir site
ee site create example.com --type=wp --mu=subdir

# Create WordPress multisite subdom site
ee site create example.com --type=wp --mu=subdom

# Create WordPress site with ssl from letsencrypt
ee site create example.com --type=wp --ssl=le

# Create WordPress site with wildcard ssl
ee site create example.com --type=wp --ssl=le --wildcard

# Create WordPress site with self signed certificate
ee site create example.com --type=wp --ssl=self

# Create WordPress site with remote database
ee site create example.com --type=wp --dbhost=localhost --dbuser=username --dbpass=password

# Create WordPress site with custom site title, locale, admin user, admin email and admin password
ee site create example.com --type=wp --title=easyengine  --locale=nl_NL --admin-email=easyengine@example.com --admin-user=easyengine --admin-pass=easyengine
```

### Options

| Argument                      | Description                                               |
|:------------------------------|:----------------------------------------------------------|
| `<site-name>`                 | Name of website                                           |
| `--cache`	                    | Use redis cache for PHP                                   |
| `--vip`	                    | Create WordPress VIP GO site using your vip repo          |
| `--mu=<subdir>`	            | WordPress sub-dir Multi-site                              |
| `--mu=<subdomain>`	        | WordPress sub-domain Multi-site                           |
| `--admin-email=<admin-email>` | E-Mail of the administrator.                              |
| `--admin-user=<admin-user>`   | Username of the administrator.                            |
| `--admin-pass=<admin-pass>`   | Password for the the administrator.                       |
| `--admin-email=<admin-email>` | E-Mail of the administrator.                              |
| `--with-db`                   | Create database for php site.                             |
| `--local-db`                  | Create separate db container instead of using global db   |
| `--php=<php-version>`         | PHP version for site. Currently PHP 5.6 and latest.       |
| `--dbname=<dbname>`           | Set the database name.                                    |
| `--dbuser=<dbuser>`           | Set the database user.                                    |
| `--dbpass=<dbpass>`           | Set the database password.                                |
| `--dbhost=<dbhost>`           | Set the database host. Pass value only when remote        |
| `--dbprefix=<dbprefix>`       | Set the database table prefix.                            |
| `--dbcharset=<dbcharset>`     | Set the database charset.                                 |
| `--dbcollate=<dbcollate>`     | Set the database collation                                |
| `--version=<version>`         | Select which WordPress  `latest` or `nightly`             |
| `--dbcharset=<dbcharset>`     | Set the database charset.                                 |
| `--dbcollate=<dbcollate>`     | Set the database collation                                |
| `--with-local-redis`          | Enable cache with local redis container.                  |
| `--skip-check`                | If set, the database connection is not checked.           |
| `--skip-status-check`         | Skips site status check.                                  |
| `--ssl=<value>`               | Enables ssl on site.                                      |
| `--wildcard`                  | Gets wildcard SSL                                         |
| `--force`                     | Resets the remote database if it is not empty.            |


[--skip-content]
: Download WP without the default themes and plugins.

[--skip-install]
: Skips wp-core install.


[--yes]
: Do not prompt for confirmation.

[--force]
: Resets the remote database if it is not empty.


#### Option PHP Version
5.6
{: .label .label-green }

7.2
{: .label .label-green }

Latest
{: .label .label-green }

#### Charset Database

default: `utf8mb4`

#### VIP Wordpress Skeleton

[VIP Wordpress Skeleton](https://github.com/Automattic/vip-go-skeleton.git)
