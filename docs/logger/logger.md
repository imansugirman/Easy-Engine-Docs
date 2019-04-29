---
layout: default
title: Logger
nav_order: 2
has_children: true
permalink: docs/logger
---

## Easy Engine Log
```
ee log show example.com
watching logfile example.com/logs/nginx/error.log
watching logfile example.com/logs/nginx/access.log
watching logfile example.com/logs/php/error.log
watching logfile example.com/logs/php/access.log
```

## Show all logs.
```
ee log show example.com --all
watching logfile ~/easyengine/sites/example.com/logs/nginx/access.log
watching logfile ~/easyengine/sites/example.com/logs/nginx/error.log
watching logfile ~/easyengine/sites/example.com/logs/debug.log
```

## Show debug log for site.
```
ee log show example.com --wp
watching logfile ~/easyengine/sites/example.com/logs/debug.log
```

## Parameter
```

--locale=<locale>	Locale for WordPress.
--le-mail=<le-mail>	Mail-id to be used for letsencrypt.
--[no-]color	Whether to colorize the output.
--debug[=<group>]	Show all PHP errors; add verbosity to EE bootstrap.
--quiet	Suppress informational messages.
```