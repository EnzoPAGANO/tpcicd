Jenkinsfile contient le pipeline pour cloner le dépôt git et récupérer les fichiers
l'inventaire.ini contient les éléments relatif à la VM qui a servi aux tests.
Le fichier playbook.yml contient une commande pour lancer le docker-compose.

Dans l'idéal, la tâche lancée par jenkins devrait exécuter le playbook.yml sur la machine décrite dans l'inventaire afin de lancer le déploiementdécrit dans le docker-compose.yml.
Ca ne fonctionne pas.