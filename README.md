# matrix-experiments

- Feb 14, 2018

https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04
https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04

https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-server-blocks-virtual-hosts-on-ubuntu-16-04

- Feb 15, 2018

Following: https://www.digitalocean.com/community/tutorials/how-to-install-matrix-synapse-on-ubuntu-16-04

End of Step 3: let's encrypt ...

Following: https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-16-04

How to set up a hostname with digitalocean:
https://www.digitalocean.com/community/tutorials/how-to-set-up-a-host-name-with-digitalocean

set up the 'www' subdomain this way (--? maybe I also need to set up related functionality in ngninx?) relevant tutorial is here: https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04

using nginx server blocks
https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-server-blocks-virtual-hosts-on-ubuntu-16-04

https://storrgie.epiphyte.network/running-a-matrix-homeserver/

--- Feb 18, 2018 -----

https://github.com/matrix-org/synapse

Installing prerequisites on Raspbian:

sudo apt-get install build-essential python2.7-dev libffi-dev \
                     python-pip python-setuptools sqlite3 \
                     libssl-dev python-virtualenv libjpeg-dev

sudo pip install --upgrade pip
sudo pip install --upgrade ndg-httpsclient
sudo pip install --upgrade virtualenv

virtualenv -p python2.7 ~/.synapse
source ~/.synapse/bin/activate
pip install --upgrade pip
pip install --upgrade setuptools
pip install https://github.com/matrix-org/synapse/tarball/master

Note -- cryptography build is very slow, requires significant RAM. 

See:
https://community.letsencrypt.org/t/installation-hangs-at-running-setup-py-install-for-cryptography/7202/4

takes a few minutes on a pi 3, but finished.

pynacl -- also very slow -- even longer than crypto above

did we need to do this bdist_wheel ... 

okay, so process took at least 30 minutes.

installed ufw

do we need to install nginx on rpi?
if so: https://www.raspberrypi.org/documentation/remote-access/web-server/nginx.md

nginx on digitalocean: https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04

trying to install nginx

followed the digitalocean tutorial.

https://thepi.io/how-to-set-up-a-web-server-on-the-raspberry-pi/

https://pimylifeup.com/raspberry-pi-ssl-lets-encrypt/

raspberry pi 3 as access point: https://www.raspberrypi.org/documentation/configuration/wireless/access-point.md

using a raspberry pi as a server:
https://www.toptal.com/raspberry-pi/how-to-turn-your-raspberry-pi-into-a-development-server

https://opensource.com/article/17/3/building-personal-web-server-raspberry-pi-3

https://www.linux.com/blog/3-ways-run-remote-desktop-raspberry-pi

https://frillip.com/using-your-raspberry-pi-3-as-a-wifi-access-point-with-hostapd/


