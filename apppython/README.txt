Le dockerfile contient les infos pour build l'image via la commande : docker build -t pythonapp:1.0  Installe au passage flask pour héberger l'appli depuis requirements.txt
main.py contient le code de l'appli.
docker-compose.yml gère le déploiements de 3 pods de l'appli python, grace à un template, et utilise ingress pour gérer les différentes URL d'accès au différents environnments.

Dans l'idéal, une fois l'image créée, on devrait pouvoir lancer les pods avec docker-compose apply -f docker-compose.yml, et accéder à l'appli aux différentes URL sur le port 3800, mais ça marche pas.
