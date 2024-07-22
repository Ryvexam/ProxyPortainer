# 📡 Guide de Connexion et Installation sur un Serveur Linux Debian 12

## 🔑 Connexion SSH au Serveur

1. **Ouvrez votre terminal et connectez-vous en SSH**:
   ```sh
   ssh utilisateur@ip_du_serveur
   ```

## ⬆️ Mise à Jour du Système

2. **Mettez à jour et upgradez votre système**:
   ```sh
   sudo apt update && sudo apt upgrade -y
   ```

## 🐳 Installation de Docker et Docker Compose

3. **Installez Docker**:
   ```sh
   sudo apt install docker.io -y
   ```

4. **Installez Docker Compose**:
   ```sh
   sudo apt install docker-compose -y
   ```

## 📥 Cloner le Répôt Git et Lancer Docker Compose

5. **Clonez le répertoire git actuel à la racine**:
   ```sh
   git clone https://github.com/Ryvexam/ProxyPortainer
   ```

6. **Accédez au dossier cloné `ProxyPortainer`**:
   ```sh
   cd ProxyPortainer
   ```

7. **Lancez Docker Compose**:
   ```sh
   docker-compose up -d
   ```

## 🌐 Accès aux Interfaces Web

8. **Connectez-vous à l'IP du serveur sur le port par défaut de Portainer (9000)**:
   ```plaintext
   http://ip_du_serveur:9000
   ```

9. **Entrez les identifiants souhaités (sécurisés !!)**.

10. **Faites de même pour Nginx Proxy Manager (port par défaut 81)**:
    ```plaintext
    http://ip_du_serveur:81
    ```

11. **Connectez-vous avec les identifiants par défaut**:
    - 📧 Email: `admin@example.com`
    - 🔒 Mot de passe: `changeme`

    ⚠️ **Changez impérativement ces identifiants par défaut !**

## 🌍 Création et Gestion des Sous-Domaines

12. **Créer les sous-domaines souhaités et les rediriger vers le serveur**.

13. **Gérer et manager les redirections et containers depuis les interfaces web**.

---

🎉 Vous avez terminé ! Votre serveur est maintenant prêt à être utilisé avec Docker et Docker Compose pour gérer vos containers et redirections.
