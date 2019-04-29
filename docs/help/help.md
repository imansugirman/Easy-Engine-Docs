---
layout: default
title: Help
nav_order: 7
has_children: true
permalink: docs/help
---

## Easy Engine Help

Get help on EE, or on a specific command.

### ee help

```
# get help for `site` command
ee help site

# get help for `site create` subcommand
ee help site create
```

### Global Parameter

| Argument              | Description                                           |
|:----------------------|:------------------------------------------------------|
| `--sites_path=<path>` | Absolute path to where all sites will be stored       |
| `--locale=<locale>`	| Locale for WordPress                                  |
| `--le-mail=<le-mail>` | Mail-id to be used for letsencrypt                    |
| `--[no-]color`        | Whether to colorize the output.                       |
| `--debug[=<group>]`   | Show all PHP errors; add verbosity to EE bootstrap.   |
| `--quiet`             | Suppress informational messages                       |
