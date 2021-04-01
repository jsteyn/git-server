# git server

Recipe to setup a git server on your Raspberry Pi. This is a part of the [CarpenPi](https://github.com/CarpenPi) project, which aims to bring [Software Carpentries](https://carpentries.org) to the Raspberry Pi, for use in off-grid and resource constrained environments.

* You'll need a Raspberry Pi 4 to setup Gitlab, with ssh setup
* Login to the Raspberry Pi https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md
(If ssh is not running, and it says "connection refused", run this on the Pi `systemctl start ssh` to enable SSH.

* Then follow the instructions here (estimated time ~5-10min): 
https://about.gitlab.com/install/#raspberry-pi-os
Ensure to select all defaults when prompted at the Postfix stage, but run `sudo apt-get install gitlab-ce` instead of `sudo EXTERNAL_URL="https://gitlab.example.com" apt-get install gitlab-ce`.
