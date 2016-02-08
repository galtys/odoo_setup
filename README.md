EASY SUDO
---------

```
cat >> /etc/sudoers.d/openerp
openerp ALL=NOPASSWD: ALL

chmod 440 /etc/sudoers.d/openerp
```

SETUP
-----

```
sudo apt-get -y  install git openssh-server postgresql emacs
sudo apt-get -y install python-pip
sudo apt-get -y install bzr
sudo pip install simple-crypt
sudo pip install --upgrade simple-crypt
sudo pip install -U  oerplib
sudo aptitude install -y python-mako

mkdir github.com
cd ./github.com
git clone https://github.com/galtys/odoo_setup.git
cd ./odoo_setup
./install.sh
```

SETUP GOLIVE
------------

```
cd ~/github.com
git clone https://github.com/galtys/gtc.git
cd ./gtc
sudo python setup.py install
```

DISABLE SUDO
------------

```
rm /etc/sudoers.d/openerp
```