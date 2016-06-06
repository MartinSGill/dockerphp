# Docker php

Followed a great tutorial at [osteel's blog](1), but it didn't work when
using docker-machine and windows.

I had to wrap it in a vagrant project to properly be able to map the local
dev folder into the VM.

Side effect is that you don't need docker installed locally at all now, just
vagrant.

Usage:

* Install VirtualBox
* Install vagrant
* Install docker-compose plugin
  * vagrant plugin install vagrant-docker-compose
* `vagrant up`

http://localhost:8080 is the source
http://localhost:8081 is phpMyAdmin

_Note:_ because the data containers are local, you'll not have all the data
and will need to add it again yourself.

[1]: http://blog.osteel.me/posts/2015/12/18/from-vagrant-to-docker-how-to-use-docker-for-local-web-development.html
