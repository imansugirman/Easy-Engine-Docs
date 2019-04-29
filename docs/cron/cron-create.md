---
layout: default
title: Crone Create
parent: Cron Job
nav_order: 2
---

## Easy Engine Create Crone

Adds a cron job to run a command at specific interval etc.

```
# Adds a cron job on example.com every 10 minutes
ee cron create example.com --command='wp cron event run --due-now' --schedule='@every 10m'

# Adds a cron job on example.com every 1 minutes
ee cron create example.com --command='wp cron event run --due-now' --schedule='* * * * *'

# Adds a cron job on example.com every 1 minutes run as user www-data
ee cron create example.com --command='wp cron event run --due-now' --schedule='* * * * *' --user=www-data

# Adds a cron job to host running EasyEngine
ee cron create host --command='wp cron event run --due-now' --schedule='@every 10m'

# Adds a cron job to host running EasyEngine
ee cron create host --command='wp media regenerate --yes' --schedule='@weekly'
```

### Options

| Argument                      | Description                                               |
|:------------------------------|:----------------------------------------------------------|
| `<site-name>`                 | Name of site to run cron on.                              |
| `--command=<command>`	        | Command to schedule.                                      |
| `--schedule=<schedule>`       | Time to schedule. Format is same as Linux cron            |
| `--user=<user>`               | User to execute command as                                |

We also have helper to easily specify scheduling format:

| Argument                      | Description                                    | Equivalent To
|:------------------------------|:-----------------------------------------------|:-------------
| `@yearly (or @annually)`      | Run once a year, midnight, Jan. 1st            | `0 0 1 1 *`
| `@monthly`	                | Run once a month, midnight, first of month.    | 	`0 0 1`
| `@weekly`                     | Run once a week, midnight between Sat/Sun      |  `0 0 0`
| `@daily (or @midnight)`       | User to execute command as                     |

You may also schedule a job to execute at fixed intervals, starting at the time it's added or cron is run. This is supported by following format:

`@every <duration>`

Where duration can be combination of:
* `<number>h - hour`
* `<number>m - minute`
* `<number>s - second`

So `1h10m2s` is also a valid duration

