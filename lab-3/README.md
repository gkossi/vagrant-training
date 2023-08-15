# VAGRANT-TRAINING / Module 04  Vagrantfile
----------------------------------------------------------------------

# Lab-3 : Création d'un Vagrantfile
- Créez un dossier lab-3
- Déplacez-vous dans ce dossier
- Initialisez vagrant afin de configurer la Vm à partir des informations suivantes :
    . Image de base : Centos 7 By Geerlingguy
    . CPU : 2
    . RAM : 2 Go
- Variabilisez les paramètres indiquées ci-dessus
- Connecter-vous en ssh
- Installer nginx
- Arretez la VM puis supprimez-là

# Commandes à utiliser

- Créez un dossier lab-3
mkdir lab-3

- Déplacez-vous dans ce dossier
cd lab-3

- Initialisez vagrant afin de configurer la Vm à partir des informations suivantes :
Image de base : Centos 7 By Geerlingguy
CPU : 2
RAM : 2 Go

- Aller sur Vagrant cloud, créer un compte et se connecter
- Rechercher centos 7 pour virtualbox créée par geerlingguy
vagrant init geerlingguy/centos7 -m

- Variabilisez les paramètres indiquées ci-dessus

- Démarrer la VM
vagrant up

- Connecter-vous en ssh
vagrant ssh

- Installer nginx
sudo apt-get update
sudo apt-get install nginx -y

sudo service nginx start

création de vbox : vagrant package --output nginx.box
créer un compte sur vagrant cloud et publier la vbox

- Arretez la VM puis supprimez-là
* arreter: vagrant halt
* supprimer: vagrant destroy