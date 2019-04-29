---
layout: default
title: Shell
nav_order: 5
has_children: true
permalink: docs/shell
---

## Easy Engine Shell

Brings up a shell to run wp-cli, composer etc.

```
# Open shell for site
$ ee shell example.com

# Open shell with root user
$ ee shell example.com --user=root

# Open shell for some other service
$ ee shell example.com --service=nginx

# Run command non-interactively
$ ee shell example.com --service=nginx --command='nginx -t &amp;&amp; nginx -s reload'
```

### Option

| Argument              | Description                                           |
|:----------------------|:------------------------------------------------------|
| `<site-name>`         | Name of website to run shell on                       |
| `--user=<user>`	    | Set the user to exec into shell                       |
| `--service=<service>` | Set the service whose shell you want default `php`    |
| `--command=<command>` | Command to non-interactively run in the shell         |



### Global Parameter

| Argument              | Description                                           |
|:----------------------|:------------------------------------------------------|
| `--sites_path=<path>` | Absolute path to where all sites will be stored       |
| `--locale=<locale>`	| Locale for WordPress                                  |
| `--le-mail=<le-mail>` | Mail-id to be used for letsencrypt                    |
| `--[no-]color`        | Whether to colorize the output.                       |
| `--debug[=<group>]`   | Show all PHP errors; add verbosity to EE bootstrap.   |
| `--quiet`             | Suppress informational messages                       |
