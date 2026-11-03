# ALCASAR Connect

**by Subaru-Kuzuky** · Windows 10/11 · PowerShell 5.1 · Open source

Application graphique de connexion automatique aux portails captifs ALCASAR (CoovaChilli). Interface sombre, configuration du Wi-Fi (SSID), de l'identifiant et du mot de passe, bouton de test, journal d'activité et automatisation silencieuse via le Planificateur de tâches Windows.

## Installation

1. Télécharger le pack de la version 1.2 et extraire tout son contenu.
2. Exécuter `INSTALLER.cmd`.
3. Dans **ALCASAR Connect**, renseigner son propre SSID, identifiant et mot de passe, puis cliquer **Enregistrer**.
4. Utiliser **Tester maintenant** puis **Actualiser** pour lire le résultat.

L'application s'installe sous `%LOCALAPPDATA%\ALCASAR-AutoLogin`. Le moteur s'exécute au démarrage de session et vérifie l'accès toutes les deux minutes.

## Sécurité

**Ne jamais publier `config.json`**, qui contient localement les identifiants, y compris le mot de passe en clair. Seul `config.example.json` doit être versionné. Les journaux peuvent également contenir des détails réseau. Le programme emploie un contournement de validation TLS pour des portails locaux : utiliser uniquement sur un réseau de confiance et demander à son administrateur de renouveler les certificats expirés.

L'application n'est **pas officielle** et n'est pas compatible avec toutes les variantes ALCASAR. Ne l'utiliser que sur les réseaux auxquels vous êtes autorisé à vous connecter.

## Sources

Le pack 1.2 comprend `AutoLogin.ps1`, `Interface.ps1`, `Installer.ps1`, les lanceurs CMD/VBS et les icônes ICO/PNG. **Les sources complètes restent à importer dans ce dépôt.**

## Crédits

Auteur : **Subaru-Kuzuky**. Assistance au développement : OpenAI ChatGPT.

Licence MIT — voir `LICENSE`.
