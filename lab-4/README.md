# VAGRANT-TRAINING / Module 05 Networking
----------------------------------------------------------------------

# Lab-4 : Déploiement d'un serveur web
- Créez un dossier lab-4
- Déplacez-vous dans ce dossier
- Créer un vagrantfile afin de configurer la VM à partir des informations suivantes :
    . Image de base => Centos 7 By Geerlingguy,
    . CPU => 2,
    . RAM => 2 Go
    . IP fixe privé : 10.0.0.10
- Variabilisez les paramètres indiquées ci-dessus
- Connecter-vous en ssh
- Installer nginx
- Vérifier que vous avez accès à l'application depuis le PC local vis http://10.0.0.10
- Arretez la VM puis supprimez-là

# Commandes à utiliser

- Créez un dossier lab-3 : mkdir lab-4

- Déplacez-vous dans ce dossier : cd lab-4

- Initialisez vagrant afin de configurer la Vm à partir des informations suivantes :
    . Image de base => Centos 7 By Geerlingguy,
    . CPU => 2,
    . RAM => 2 Go
    . IP fixe privé : 10.0.0.10

- Aller sur Vagrant cloud, créer un compte et se connecter
- Rechercher centos 7 pour virtualbox créée par geerlingguy : vagrant init geerlingguy/centos7 -m

- Valider le fichier Vagrantfile (à faire à chaque modification du fichier Vagrantfile) : vagrant validate

- Variabilisez les paramètres indiquées ci-dessus

- Démarrer la VM : vagrant up

- Connecter-vous en ssh : vagrant ssh

- Installer nginx : sudo apt-get update ; sudo apt-get install nginx -y

sudo service nginx start

- création de vbox : vagrant package --output nginx.box
- créer un compte sur vagrant cloud et publier la vbox

- Arretez la VM puis supprimez-là :
* arreter : vagrant halt
* supprimer : vagrant destroy