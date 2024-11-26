# TP Linux

## Architecture du TP
- /manager : Contient le conteneur qui va gérer le serveur avec :
  - traefik : Routeur et reverse proxy
  - prometheus : Monitoring et métriques
  - grafana : Visualisation de données métriques, monitoring
  - docker-compose.yml
- /project : Contient un projet de test PHP :
  - index.php
  - docker.compose.yml

## Procédure
- apt update && apt upgrade
- passwd
- nano /etc/ssh/sshd_config :
  - Port 8121
  - AllowUsers nicolas
  - PermitRootLogin no
- adduser nicolas
- usermod -aG sudo nicolas
- Ajout de l'utilisateur au fichier /etc/sudoers :
  - nano /etc/sudoers
- Installation de fail2ban
- Configuration du Firewall Nftables
- Installation de docker
- Installation de ctop
