The Hit List
============

A list of projects, solutions, guidelines, source code, gists for common and not-so-common problems.

Server Side (self contained services and libraries)
---------------------------------------------------

Shell Wrapping:

http://symfony.com/doc/current/components/process.html
https://github.com/adambrett/php-shell-wrapper
https://github.com/MrRio/shellwrap
https://github.com/arturadib/shelljs (port this over to PHP or use Node.js RPC)

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

Collections
Ardent https://github.com/morrisonlevi/Ardent

Memory Management
https://github.com/zendframework/Component_ZendMemory (http://framework.zend.com/manual/1.12/en/zend.memory.overview.html)
http://www.php.net/manual/en/internals2.memory.php
Important for Daemons!

### Fault Tolerant Programming

https://github.com/odesk/phystrix (inspired by https://github.com/Netflix/Hystrix)
https://github.com/asm89/php-try

Client Side
-----------

### Charting

NVD3.js
Morris charts
Dygraphs.com

### UI Frameworks

Bootstrap
Foundation
Semantic UI
Ionic

### AJAX File Downloading

http://stackoverflow.com/questions/16514509/how-do-you-serve-a-file-for-download-with-angularjs-or-javascript

http://jsfiddle.net/g/CncFy/

http://davidwalsh.name/download-attribute

CLI Tools
---------

### Watching

https://github.com/EHER/phpwatch (Any system but very slow)
https://github.com/facebook/watchman (only for Unixy systems)

### CLI User Interface Tools

https://github.com/zetacomponents/ConsoleTools

### Framework

http://symfony.com/doc/current/components/console/introduction.html

Development Tools
-----------------

GUI for X Certificate and Key Management. Like your own little CA for self signed SSL certificates: http://sourceforge.net/projects/xca/ (cross platform)

GUI Hosts File Editor: http://hostsfileeditor.codeplex.com/ (Windows)

CRLF to LF - dos2unix (Some conf files need LF)

### Version Managers

PHP - phpbrew https://github.com/c9s/phpbrew
Python - virtualenv
Ruby - rvm
Node - n

### Phars

https://github.com/kherge/php-box

### LocalHost Tunnelling

https://ngrok.com/
https://github.com/inconshreveable/ngrok

### Package Managers

pulldown - random text files and etc!
all the others
browserify
webpack
and the combiner (writes json files for all those package managers)

### Service Oriented Architecture

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

Statistics Collection Service - Collectd will soon include https://github.com/etsy/statsd/

Source Code Control (Gitlab)

### Virtual Appliance Creation Useful for Service Oriented Architectures

1. http://www.packer.io/ (Supports all cross-platform VA formats AND Docker)
2. Use Dockerfiles directly (but then can only support docker!)

See:
https://gitlab.com/gitlab-org/gitlab-packer/tree/master
http://mmckeen.net/blog/2013/12/27/advanced-docker-provisioning-with-packer/
http://mmckeen.net/blog/2013/12/14/docker-all-the-things-nginx-and-supervisor/

### Provisioners

Use ANSIBLE!!

### Dev Environments

Use Packer to create standardised base boxes for development. (For Vagrant + Targetted Host (DigitalOcean))
(Packer will use Ansible as provisioners and config management)

VirtualBox + Vagrant + Docker uses these base boxes, and you build your app in these environments.

Once the app is developed, use Packer (along with additional Ansible) to build a new box as a virtual software appliance and then deploy it.

Deploy it on the Matrix as a Docker container.

https://groups.google.com/forum/#!msg/packer-tool/4lB4OqhILF8/NPoMYeew0sEJ


OR

Packer with Ansible creates a Vagrant Box that supports Docker and Other Common Dev things.

Vagrant runs this new vagrant box. You develop on it.

Then use Packer to package up the developed docker container.

pretengineer.com/post/packer-vagrant-infra

http://mmckeen.net/blog/2013/12/27/advanced-docker-provisioning-with-packer/

### DVCS Workfow

https://github.com/gushphp/gush for Git/Github management

### Editors

Sublime Text Editor (or https://github.com/limetext/lime)

 - https://github.com/SublimeLinter/SublimeLinter3

### API Documentation Generators

PHPDocumentor for PHP