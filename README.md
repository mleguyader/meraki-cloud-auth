# Meraki Cloud Auth

Portail web moderne pour gérer les utilisateurs d'un réseau WiFi Meraki avec authentification cloud.

## Fonctionnalités

- Création manuelle ou en batch d'utilisateurs avec expiration
- Authentification admin via LDAP
- Dashboard interactif (recherche, pagination)
- Alertes email automatiques pour les expirations
- Export CSV automatique par email
- Téléchargement des logs
- Déploiement complet via Docker

## Déploiement rapide

```bash
git clone https://github.com/ton-utilisateur/meraki-cloud-auth.git
cd meraki-cloud-auth
cp .env.example .env
docker build -t meraki-cloud-auth .
docker run -d --restart=always --env-file .env -p 5000:5000 meraki-cloud-auth
```

Accéder à http://localhost:5000

## Exemple de fichier .env

Voir `.env.example`
