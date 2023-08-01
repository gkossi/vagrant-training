# VAGRANT-TRAINING


----------------------------------------------------------------------
# TP N°2/Lab-2 : Créer un vbox
----------------------------------------------------------------------
- Créez un dossier Lab-2
- Déplacez-vous dans ce dossier
- Initialisez vagrant en utilisant la version 20190425.0.0 ubuntu/trusty64 (vagrant init ubuntu/trusty64)
- Démarrer la VM (vagrant up)
- Connecter-vous en ssh (vagrant ssh)
- Installer nginx
- Démarrer le service et activez son démarrage au lancement de la VM
- Créez une vbox à parti de cette VM
- Créez un compte sur vagrant cloud
- Publiez votre vbox sur vagrant cloud sous le nom <username>/nginx en version v1
- Arretez la VM puis supprimez-là (vagrant destroy)

----------------------------------------------------------------------
# Commandes à utiliser
----------------------------------------------------------------------
* mkdir Lab-2
* cd Lab-2
* vagrant init ubuntu/trusty64 --box-version 20190425.0.0
* vagrant up
* vagrant ssh
* sudo apt-get update; sudo apt-get install nginx -y
* sudo service nginx start
* création de vbox : vagrant package --output nginx.box
* créer un compte sur vagrant cloud et publier la vbox
* arreter: vagrant halt
* supprimer: vagrant destroy