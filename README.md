# git server

Recipe to setup a git server on your Raspberry Pi. 

This is a part of the [CarpenPi](https://github.com/CarpenPi) project, which aims to bring [Software Carpentries](https://carpentries.org) to the Raspberry Pi, for use in off-grid and resource constrained environments.

We'll be using the [Gitea](https://gitea.io) server which is easy to install (it's a single file binary). Setting up Gitea allows participants to manage repositories for
using a local network connection, rather than through a website interface
connected to the Internet.

* You'll need a Raspberry Pi 4 to setup Gitea, with ssh setup
* Login to the Raspberry Pi https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md
(If ssh is not running, and you get the error "Connection refused", run this on the Pi `systemctl start ssh` to enable SSH)

* Then follow the instructions here (estimated time ~5-10min): 
https://docs.gitea.io/en-us/install-from-binary/
* Get the IP address of the Pi using this command
    ```hostname -I```
* Connect to `http://localhost:3000/` on your Pi or `http://IPADDRESS-HERE:3000/`
