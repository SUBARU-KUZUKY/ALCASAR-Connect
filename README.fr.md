# ALCASAR Connect 🇫🇷

**by Subaru-Kuzuky** · Windows 10/11 · PowerShell 5.1 · Licence MIT

[English](README.en.md) | [Accueil](README.md)

## Présentation
Logiciel Windows non officiel pour se connecter automatiquement aux portails captifs ALCASAR / CoovaChilli sur un réseau autorisé. Interface graphique sombre, Wi-Fi configurable, identifiants modifiables, test manuel, automatisation silencieuse et journal de connexion.

## Installation et test
La documentation est publiée, mais les sources complètes et la Release téléchargeable **ne sont pas encore sur GitHub**. En attendant, le pack de test peut être utilisé localement.

1. Extraire le pack complet.
2. Lancer `INSTALLER.cmd` sur Windows.
3. Entrer le SSID et **ses propres identifiants** dans l'interface ; cliquer sur **Enregistrer**.
4. Tester la connexion et consulter le journal avec **Actualiser**.

Le dossier d'installation prévu est `%LOCALAPPDATA%\ALCASAR-AutoLogin`. La tâche automatique peut contrôler la connexion toutes les deux minutes.

## Sécurité
Ne jamais publier `config.json`, les mots de passe ou des journaux contenant des données sensibles. Le moteur utilise actuellement des requêtes avec désactivation de la vérification des certificats TLS locaux : uniquement sur un réseau de confiance, en attendant que l'administrateur corrige les certificats. Logiciel non officiel, compatibilité variable selon les portails, et à utiliser uniquement avec autorisation.

## Crédits
**Développé par Subaru-Kuzuky** · Assistance technique : **OpenAI**.

Licence [MIT](LICENSE). Contributions bienvenues une fois les sources publiées.
