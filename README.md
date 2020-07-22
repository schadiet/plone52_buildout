# plone52_buildout

Installation procedure for the Plone-Installation of Udemy Course - Plone CMS: Programming Add-ons with Python

Installation
============

Preparation of the Ubuntu-Systems
-------------------------------

Update your Packagemanager
* sudo apt-get update

Installing Dependencies
* sudo apt-get install build-essential python-dev libjpeg-dev libxslt-dev supervisor
* sudo apt-get install libpython3-dev
* sudo apt-get install python3-pip


Binaries to indexing the Content
-----------------------------------

* sudo apt-get install wv
* sudo apt-get install poppler-utils
* sudo apt-get install htop
* sudo apt-get install git

Update again
* sudo apt-get update

More Dependencies
* sudo apt-get install gcc libpq-dev libffi-dev libssl-dev -y
* sudo apt-get install python-dev  python-pip -y
* sudo apt-get install python3-dev python3-pip python3-venv python3-wheel -y
* sudo apt-get install libsasl2-dev python-dev libldap2-dev libssl-dev

Preparation and Execution of Plon-Buildout
-------------------------------------------------

* ~ > git clone https://github.com/schadiet/plone52_buildout.git $projectname
* ~ > cd $projectname
* ~/$projectname > python3 -m venv .
* ~/$projectname > ./bin/pip install -r requirements.txt
* ~/$projectname > ./bin/buildout

Buildout with Developer-Tools
----------------------------
* ~/$projectname > ./bin/buildout -c develop.cfg

Customization of buildout.cfg after git clone
-----------------------------------------

* user=admin:admin
* buildout-user = codingsolo
* ports of clients
