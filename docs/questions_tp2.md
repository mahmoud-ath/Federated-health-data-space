## TP 2 — Réponses aux questions

1. **Quel est le rôle de FastAPI ?**

   FastAPI permet de créer des API REST pour exposer les données des deux organisations et les rendre accessibles à distance.

2. **Quel est le rôle de Uvicorn ?**

   Uvicorn est un serveur qui exécute l'application FastAPI et permet aux clients de communiquer avec elle via HTTP.

3. **Pourquoi utilise-t-on deux ports différents ?**

   Pour exécuter les deux API simultanément sans conflit : le port 8001 pour l'environnement et le port 8002 pour l'hôpital.

4. **Le laboratoire reçoit-il les données brutes dans cette version ?**

   Oui. Le client du laboratoire récupère les données brutes des deux API au format JSON pour effectuer les analyses localement.

5. **Une API REST garantit-elle automatiquement la confidentialité ?**

   Non. Une API REST ne garantit pas automatiquement la confidentialité. Il faut ajouter des mécanismes de sécurité comme l'authentification, l'autorisation et le chiffrement HTTPS.