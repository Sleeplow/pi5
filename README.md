# pi5.sleeplow.ca

Clé **publique** de l'intégration Tesla Fleet de Home Assistant (homelab Raspberry Pi 5),
publiée à `https://pi5.sleeplow.ca/.well-known/appspecific/com.tesla.3p.public-key.pem`.

La clé privée reste sur le Pi. `.nojekyll` est nécessaire pour publier le dossier `.well-known`.

`go.html` : relais pour l'app iPhone du tableau de bord. iOS n'envoie vers Safari que des adresses HTTPS
(`x-safari-https://`) ; l'app ouvre donc `https://pi5.sleeplow.ca/go.html#<adresse>`, qui redirige vers
l'adresse du réseau privé (192.168.x, 10.x, 100.64-127.x). L'adresse après le `#` n'est jamais envoyée au serveur.
