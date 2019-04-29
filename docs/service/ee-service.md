---
layout: default
title: Service
nav_order: 3
has_children: true
permalink: docs/service
---

## Easy Engine Service

### Restart Command 

```
# Restarts global nginx proxy service
ee service restart nginx-proxy
```

### Disable Command 

```
# Disable global service
$ ee service disable nginx-proxy
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
