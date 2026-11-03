# ALCASAR Connect 🇫🇷

**by Subaru-Kuzuky** · Windows 10/11 · PowerShell 5.1 · Open source

[English](README.en.md) | [Accueil / Home](README.md)

## Présentation

**ALCASAR Connect** est un outil non officiel pour Windows qui automatise la connexion à un portail captif **ALCASAR / CoovaChilli** sur un réseau auquel vous êtes autorisé à accéder.

L'application propose une interface sombre, un SSID Wi-Fi configurable, des champs d'identifiant et de mot de passe, un bouton de test, un journal d'activité et une tâche planifiée qui vérifie périodiquement la connectivité.

## Fonctionnalités

- Interface graphique sous Windows
- Paramétrage du réseau Wi-Fi (SSID), de l'identifiant et du mot de passe
- Test manuel de l'authentification
- Vérification automatique en arrière-plan à l'ouverture de session et toutes les deux minutes
- Journal de diagnostic
- Raccourcis Bureau et menu Démarrer

## Installation

> **État du dépôt :** la documentation et un exemple de configuration sont publiés, mais les **sources complètes de l'application doivent encore être importées**. Il n'y a pas encore de Release GitHub vérifiée pour une installation directe.

Une fois le pack complet disponible :

1. Télécharger l'archive de la version publiée et l'extraire entièrement.
2. Exécuter `INSTALLER.cmd` sur Windows.
3. Ouvrir **ALCASAR Connect** et saisir ses **propres identifiants** et le SSID du réseau.
4. Cliquer sur **Enregistrer**, puis sur **Tester maintenant**.
5. Examiner le journal avec **Actualiser** pour vérifier le résultat.

L'installation prévue utilise le dossier `%LOCALAPPDATA%\ALCASAR-AutoLogin`.

## Sécurité et confidentialité

- **Ne publiez jamais `config.json`**, qui peut contenir un mot de passe en clair.
- Utilisez le fichier `config.example.json` comme exemple uniquement.
- Les journaux peuvent contenir des renseignements sur votre réseau ; relisez-les avant de les partager.
- Certaines configurations du moteur historique désactivent la vérification TLS pour le portail local. Ce n'est pas recommandé sur un réseau non fiable : demandez à l'administrateur de renouveler les certificats expirés.
- L'application ne doit pas servir à contourner les restrictions d'un réseau ni à se connecter sans autorisation.
- Compatibilité variable selon les versions et configurations du portail ALCASAR.

## Développement et contribution

Les contributions, corrections et propositions d'amélioration sont les bienvenues après publication des sources. Pour signaler un dysfonctionnement, précisez la version du logiciel, la version de Windows et les messages de diagnostic, **sans divulguer de mot de passe**.

## Crédits et licence

**Auteur : Subaru-Kuzuky**

Assistance au développement : OpenAI ChatGPT.

Projet indépendant, non affilié à l'équipe officielle d'ALCASAR. Licence [MIT](LICENSE).
