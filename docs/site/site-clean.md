---
layout: default
title: Easy Engine Site Clean
parent: Site
nav_order: 2
---

## Easy Engine Site Clean

```
# Clear Both cache type for site.
$ ee site clean example.com

# Clear Object cache for site.
$ ee site clean example.com --object

# Clear Page cache for site.
$ ee site clean example.com --page
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
