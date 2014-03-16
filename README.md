The Hit List
============

A list of projects, solutions, guidelines, source code, gists for common and not-so-common problems.

Server Side (self contained services and libraries)
---------------------------------------------------

Shell Wrapping:

https://github.com/adambrett/php-shell-wrapper
https://github.com/MrRio/shellwrap

Notificator:

https://github.com/namshi/notificator

Async Frameworks:
https://github.com/rdlowrey/Amp
React

IOC
https://github.com/rdlowrey/Auryn

HTTP Client
Requests (Flexible, good for small libraries, Easiest to learn (does not need curl but can use it to allow async, otherwise fallsback on fsockopen))
Artax (Best for Async or Low level connections (does not need curl))
Guzzle (Most Featured (needs curl))

Client Side
-----------

### Charting

NVD3.js
Morris charts
Dygraphs.com

Development Tools
-----------------

GUI for X Certificate and Key Management. Like your own little CA for self signed SSL certificates: http://sourceforge.net/projects/xca/ (cross platform)

GUI Hosts File Editor: http://hostsfileeditor.codeplex.com/ (Windows)

CRLF to LF - dos2unix (Some conf files need LF)

Versoin Managers
---------------

PHP - phpbrew https://github.com/c9s/phpbrew
Python - virtualenv
Ruby - rvm
Node - n

Phars
-----

https://github.com/kherge/php-box

LocalHost Tunnelling
--------------------

https://ngrok.com/
https://github.com/inconshreveable/ngrok

Package Managers
----------------

pulldown - random text files and etc!
all the others
browserify
webpack
and the combiner (writes json files for all those package managers)

Service Oriented Architecture
-----------------------------

Event Bus (MQ)

Notificator

Relay

Auth (Identity Service)

Chat

Batch Processing

RPC

Logging

Scheduler - Chronus

Monitoring - Circus

Deployment - Rocketeer

Hosting - Matrix Cloud

Source Code Control (Gitlab)

Virtual Appliance Creation Useful for Service Oriented Architectures
--------------------------------------------------------------------

1. http://www.packer.io/ (Supports all cross-platform VA formats AND Docker)
2. Use Dockerfiles directly (but then can only support docker!)

See:
https://gitlab.com/gitlab-org/gitlab-packer/tree/master
http://mmckeen.net/blog/2013/12/27/advanced-docker-provisioning-with-packer/
http://mmckeen.net/blog/2013/12/14/docker-all-the-things-nginx-and-supervisor/

Provisioners
------------

Use ANSIBLE!!