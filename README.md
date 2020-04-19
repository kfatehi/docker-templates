# Unraid Templates
- [CyberChef](#cyberchef)
- [Dashmachine](#dashmachine)
  * [Default username and password](#default-username-and-password)
  * [~~Unauthorized~~](#unauthorized)
- [db-backup](#db-backup)
  * [Environment Variables](#environment-variables)
- [ddns-route53](#ddns-route53)
  * [Before running the docker](#before-running-the-docker)
- [Docpht](#docpht)
- [Droppy](#droppy)
- [FileRun](#filerun)
  * [Default username and password](#default-username-and-password-1)
- [FreePBX](#freepbx)
  * [First installation](#first-installation)
- [Freescout](#freescout)
  * [Creating User](#creating-user)
- [Firefox-Syncserver](#firefox-syncserver)
- [Flarum](#flarum)
  * [Default username and password](#default-username-and-password-2)
  * [Notes](#notes)
- [Golinks](#golinks)
  * [Usage](#usage)
- [Gotify](#gotify)
  * [Before running the docker](#before-running-the-docker-1)
  * [Default username and password](#default-username-and-password-3)
- [Homer](#homer)
  * [Before running the docker](#before-running-the-docker-2)
- [Jitsi](#jitsi)
  * [Change appdata location](#change-appdata-location)
  * [Notes](#notes-1)
- [Kiwix-serve](#kiwix-serve)
  * [Notes](#notes-2)
  * [Content](#content)
- [Mailpile](#mailpile)
- [Matrix](#matrix)
  * [Guides](#guides)
- [Miniflux](#miniflux)
  * [Notes](#notes-3)
- [Pure-FTPd](#pure-ftpd)
  * [Notes](#notes-4)
- [Reactive-resume](#reactive-resume)
- [Riot-web](#riot-web)
  * [Before running the docker](#before-running-the-docker-3)
- [Searx](#searx)
- [Shiori](#shiori)
  * [Default username and password](#default-username-and-password-4)
  * [Notes](#notes-5)
- [StackEdit](#stackedit)
- [Wallabag](#wallabag)
  * [Default username and password](#default-username-and-password-5)
  * [PHP errors](#php-errors)
  * [Missing texture and images](#missing-texture-and-images)

----
# CyberChef
![CyberChef](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/cyberchef.png)

**Application Name:** CyberChef

**Application Site:** https://gchq.github.io/CyberChef/

**Docker Hub:** https://hub.docker.com/r/aude/cyberchef

**Github:** https://github.com/aude/cyberchef-docker

----
# Dashmachine
![Dashmachine](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/dashmachine.png)

**Application Name:** Dashmachine

**Application Site:** https://github.com/rmountjoy92/DashMachine

**Docker Hub:** https://hub.docker.com/r/rmountjoy/dashmachine/

**Github:** https://github.com/rmountjoy92/DashMachine
## Default username and password
Username: ```admin```
Password: ```admin```
## ~~Unauthorized~~
~~If you get unauthorized page add /login <- ```http://IP:PORT/login```~~

----
# db-backup
![db-backup](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/db-backup.png)

**Application Name:** db-backup

**Application Site:** https://github.com/tiredofit/docker-db-backup 

**Docker Hub:** https://hub.docker.com/r/tiredofit/db-backup/

**Github:** https://github.com/tiredofit/docker-db-backup 
## Environment Variables
| Parameter | Description |
|-----------|-------------|
| `COMPRESSION` | Use either Gzip `GZ`, Bzip2 `BZ`, XZip `XZ`, or none `NONE` - Default `GZ`
| `DB_TYPE` | Type of DB Server to backup `couch` `influx` `mysql` `pgsql` `mongo` `redis` `rethink`
| `DB_HOST` | Server Hostname e.g. `mariadb`
| `DB_NAME` | Schema Name e.g. `database`
| `DB_USER` | username for the database - use `root` to backup all MySQL of them.
| `DB_PASS` | (optional if DB doesn't require it) password for the database
| `DB_PORT` | (optional) Set port to connect to DB_HOST. Defaults are provided
| `DB_DUMP_FREQ` | How often to do a dump, in minutes. Defaults to 1440 minutes, or once per day.
| `DB_DUMP_BEGIN` | What time to do the first dump. Defaults to immediate. Must be in one of two formats
| | Absolute HHMM, e.g. `2330` or `0415`
| | Relative +MM, i.e. how many minutes after starting the container, e.g. `+0` (immediate), `+10` (in 10 minutes), or `+90` in an hour and a half
| `DB_CLEANUP_TIME` | Value in minutes to delete old backups (only fired when dump freqency fires). 1440 would delete anything above 1 day old. You don't need to set this variable if you want to hold onto everything.
| `DEBUG_MODE` | If set to `true`, print copious shell script messages to the container log. Otherwise only basic messages are printed.
| `MD5` | Generate MD5 Sum in Directory, `TRUE` or `FALSE` - Default `TRUE`
| `PARALLEL_COMPRESSION` | Use multiple cores when compressing backups `TRUE` or `FALSE` - Default `TRUE` |
| `SPLIT_DB` | If using root as username and multiple DBs on system, set to TRUE to create Seperate DB Backups instead of all in one. - Default `FALSE` |

----
# ddns-route53
![ddns-route53](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/ddns-route53.png)

**Application Name:** ddns-route53

**Application Site:** https://github.com/crazy-max/ddns-route53

**Docker Hub:** https://hub.docker.com/r/crazymax/ddns-route53/

**Github:** https://github.com/crazy-max/ddns-route53
## Before running the docker
* Create ddns-route53.yml file in /mnt/user/appdata/ddns-route53/ - https://github.com/crazy-max/ddns-route53/blob/master/doc/configuration.md

----
# Docpht
![Docpht](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/docpht.png)

**Application Name:** Docpht

**Application Site:** https://docpht.org/

**Docker Hub:** https://hub.docker.com/r/docpht/docpht/

**Github:** https://github.com/docpht/docpht

----
# Droppy
![Droppy](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/droppy.png)

**Application Name:** Droppy

**Application Site:** https://droppy.silverwind.io/

**Docker Hub:** https://hub.docker.com/r/silverwind/droppy/

**Github:** https://github.com/silverwind/droppy

----
# FileRun
![FileRun](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/filerun.png)

**Application Name:** FileRun

**Application Site:** https://filerun.com/

**Docker Hub:** https://hub.docker.com/r/afian/filerun/

**Github:** https://github.com/filerun/docker
## Default username and password
Username: ```superuser```
Password: ```superuser```

----
# FreePBX
![FreePBX](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/freepbx.png)

**Application Name:** FreePBX

**Application Site:** https://www.freepbx.org/

**Docker Hub:** https://hub.docker.com/r/tiredofit/freepbx/

**Github:** https://github.com/tiredofit/docker-freepbx/
## First installation 
* Take time be patient
* Wizard setup go to http://freepbx/admin/config.php

----
# Freescout
![freescout](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/freescout.png)

**Application Name:** Freescout

**Application Site:** https://freescout.net/

**Docker Hub:** https://hub.docker.com/r/tiredofit/freescout/

**Github:** https://www.github.com/tiredofit/docker-freescout
## Creating User
* CLI ```cd /www/html``` then ```php artisan freescout:create-user```


----
# Firefox-Syncserver
![Firefox-Syncserver](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/firefox-syncserver.png)

**Application Name:** Firefox-Syncserver

**Application Site:** https://github.com/crazy-max/docker-firefox-syncserver

**Docker Hub:** https://hub.docker.com/r/crazymax/firefox-syncserver

**Github:** https://github.com/crazy-max/docker-firefox-syncserver

----
# Flarum
![Flarum](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/flarum.png)

**Application Name:** Flarum

**Application Site:** https://flarum.org/

**Docker Hub:** https://hub.docker.com/r/crazymax/flarum/

**Github:** https://github.com/crazy-max/docker-flarum
## Default username and password
Username: ```flarum```
Password: ```flarum```
## Notes
* Make Sure the base url is right if it local use only use http://<ip>:8000 and if you are hosting it on your domain it should be http://example.com or https://example.com.

----
# Golinks
![Golinks](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/golinks.png)

**Application Name:** Golinks

**Application Site:** https://github.com/prologic/golinks

**Docker Hub:** https://hub.docker.com/r/prologic/golinks/

**Github:** https://github.com/prologic/golinks
## Usage
* https://github.com/prologic/golinks#usage
    
----
# Gotify
![Gotify](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/gotify.png)

**Application Name:** Gotify

**Application Site:** https://gotify.net/

**Docker Hub:** https://hub.docker.com/r/gotify/server/

**Github:** https://github.com/gotify/server/ 
## Before running the docker
```mkdir -p /mnt/user/appdata/gotify/config/```
```wget -O /mnt/user/appdata/gotify/config/config.yml https://raw.githubusercontent.com/gotify/server/master/config.example.yml```
## Default username and password
Username: ```admin```
Password: ```admin```
    
----
# Homer
![Homer](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/homer.png)

**Application Name:** Homer

**Application Site:** https://github.com/bastienwirtz/homer

**Docker Hub:** https://hub.docker.com/r/b4bz/homer

**Github:** https://github.com/bastienwirtz/homer
## Before running the docker
```mkdir -p /mnt/user/appdata/homer/config/```
```wget -O /mnt/user/appdata/homer/config/config.yml https://raw.githubusercontent.com/bastienwirtz/homer/master/config.yml```

----
# Jitsi
![Jitsi](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/jitsi.png)

**Application Name:** Jitsi

**Application Site:** https://jitsi.org/

**Docker Hub:** https://hub.docker.com/u/jitsi/

**Github:** https://github.com/jitsi/docker-jitsi-meet
## Change appdata location
```/mnt/user/appdata/jitsi-web``` -> ```/mnt/user/appdata/jitsi/web/```
```/mnt/user/appdata/jitsi-prosody``` -> ```/mnt/user/appdata/jitsi/prosody/```
```/mnt/user/appdata/jitsi-jvb``` -> ```/mnt/user/appdata/jitsi/jvb/```
```/mnt/user/appdata/jitsi-jicofo``` -> ```/mnt/user/appdata/jitsi/jicofo/```
## Notes
* https://github.com/jitsi/docker-jitsi-meet
* How it all work
![](https://335wvf48o1332cksy23mw1pj-wpengine.netdna-ssl.com/wp-content/uploads/2018/07/docker-jitsi-meet.png)

----
# Kiwix-serve
![Kiwix-serve](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/kiwix.png)

**Application Name:** Kiwix-serve

**Application Site:** https://www.kiwix.org/

**Docker Hub:** https://hub.docker.com/r/kiwix/kiwix-serve/

**Github:** https://github.com/kiwix/kiwix-tools
## Notes
* When using variable "DOWNLOAD" remove the link after the download so you don't re-download the same content again
## Content
For more content https://wiki.kiwix.org/wiki/Content

----
# Mailpile
![Mailpile](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/mailpile.png)

**Application Name:** Mailpile

**Application Site:** https://www.mailpile.is/

**Docker Hub:** https://hub.docker.com/r/rroemhild/mailpile/

**Github:** https://github.com/rroemhild/docker-mailpile
 
----
# Matrix
![Matrix](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/matrix.png)

**Application Name:** Matrix

**Application Site:** https://matrix.org/

**Docker Hub:** https://hub.docker.com/r/avhost/docker-matrix

**Github:** https://github.com/AVENTER-UG/docker-matrix
## Guides
* Unraid User - PSYCHOPATHiO [Guide](https://forums.unraid.net/topic/89502-support-a75g-repo/?do=findComment&comment=839576)
* More info about matrix configuration [here](https://github.com/matrix-org/synapse/blob/master/README.rst)

----
# Miniflux
![Miniflux](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/miniflux.png)

**Application Name:** Miniflux

**Application Site:** https://miniflux.app/

**Docker Hub:** https://hub.docker.com/r/miniflux/miniflux/

**Github:** https://github.com/miniflux/miniflux
## Notes
* Admin username and password is setup at in docker variables then you can change in Miniflux settings. Docker variable will be ignored when you change it inside the docker.
* PostgreSQL DB Required (Not Included)

----
# Pure-FTPd
![Pure-FTPd](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/pure-ftpd.png)

**Application Name:** Pure-FTPd

**Application Site:** https://www.pureftpd.org/project/pure-ftpd/

**Docker Hub:** https://hub.docker.com/r/crazymax/pure-ftpd/

**Github:** https://github.com/crazy-max/docker-pure-ftpd
## Notes
* Creating User use console then ```pure-pw useradd admin -u 99 -g 100 -d /home/admin -m``` then enter password of your choosing.
* https://github.com/crazy-max/docker-pure-ftpd#notes

----
# Reactive-resume
![Reactive-resume](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/reactive-resume.png)

**Application Name:** Reactive-resume

**Application Site:** https://rxresu.me/

**Docker Hub:** https://hub.docker.com/r/amruthpillai/reactive-resume/

**Github:** https://www.github.com/AmruthPillai/Reactive-Resume

----
# Riot-web
![Riot-web](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/riot-web.png)

**Application Name:** Riot-web

**Application Site:** https://riot.im/

**Docker Hub:** https://hub.docker.com/r/vectorim/riot-web/

**Github:** https://www.github.com/vector-im/riot-web
## Before running the docker
```mkdir -p /mnt/user/appdata/riot-web/config```
```wget -O /mnt/user/appdata/riot-web/config/config.json https://riot.im/develop/config.json```

----
# Searx
![Searx](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/searx.png)

**Application Name:** Searx

**Application Site:** https://github.com/asciimoo/searx

**Docker Hub:** https://hub.docker.com/r/searx/searx/

**Github:** https://github.com/asciimoo/searx
    
----
# Shiori
![Shiori](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/searx.png)

**Application Name:** Shiori

**Application Site:** https://github.com/go-shiori/shiori

**Docker Hub:** https://hub.docker.com/r/radhifadlillah/shiori/

**Github:** https://github.com/go-shiori/shiori
## Default username and password
Username: ```shiori```
Password: ```gopher```
## Notes
* Create new account inside the web gui so the default one will be removed.

----
# StackEdit
![Shiori](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/stackedit.png)

**Application Name:** StackEdit

**Application Site:** https://stackedit.io/

**Docker Hub:** https://hub.docker.com/r/qmcgaw/stackedit/

**Github:** https://github.com/qdm12/stackedit-docker

----
# Wallabag
![Wallabag](https://raw.githubusercontent.com/A75G/docker-templates/master/templates/icons/wallabag.png)

**Application Name:** Wallabag

**Application Site:** https://wallabag.org/

**Docker Hub:** https://hub.docker.com/r/wallabag/wallabag

**Github:** https://www.github.com/wallabag/docker
## Default username and password
Username: ```wallabag```
Password: ```wallabag```
## PHP errors
https://github.com/wallabag/docker/issues/185
## Missing texture and images 
Make sure the domain variable is right http://ip:6500 and if you are hosting it http://wallabag.example.com or https://wallabag.example.com.
