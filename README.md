Docker LAMP Stack
=================

Source code from the article
[How to create a docker-based LAMP stack using docker-compose on Ubuntu 18.04 Bionic Beaver Linux](https://linuxconfig.org/how-to-create-a-docker-based-lamp-stack-using-docker-compose-on-ubuntu-18-04-bionic-beaver-linux)

To run:

```
$ docker-compose up
```

Disable Apache on the Host
--------------------------

If Apache is already listening on port 80 of the host machine, it can be stopped
by running:

```
$ sudo service apache2 stop
```

To disable Apache from running at boot, use:

```
$ sudo update-rc.d apache2 disable
```

And likewise, to enable Apache to run at boot again:

```
$ sudo update-rc.d apache2 enable
```
