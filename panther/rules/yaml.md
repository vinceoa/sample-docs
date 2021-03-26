---
layout: home
title: Rules file (yaml)
nav_order: 7
permalink: /panther/rules/schedules
parent: Rules
grand_parent: Panther
---

# Rules location
Depending on which way you installed Panther there are differing locations of the rule files.

## When using [docker-compose.yml](https://github.com/OpenAnswers/panther-core/blob/master/docker-compose.yml)
  A docker volume will have been created, the name is comprised of two parts.
  
  `<directory-name>_rules_vol`

  For example if your `docker-compose.yml` is in a directory called `panther` then the docker volume will be called
  `panther_rules-vol`

## When using [app.panther.support](https://app.panther.support)
  The rules are not directly accessible to the end user.

## When running the [source code](https://github.com/OpenAnswers/panther-core) 
  The rules are located under `rules/`


# Rules format

The `server.rules.yml` has three main sections

```yaml
globals:

groups:

schedules:
```
  
