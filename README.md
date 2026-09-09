# Retouch Launcher

[![Release](https://img.shields.io/github/v/release/Retouch-blog/retouch-releases?label=derni%C3%A8re%20version)](https://github.com/Retouch-blog/retouch-releases/releases/latest)
[![Downloads](https://img.shields.io/endpoint?url=https://retouch.blog/api/downloads.php&style=flat)](https://retouch.blog/#telecharger)
[![Windows](https://img.shields.io/badge/Windows-blue)](https://github.com/Retouch-blog/retouch-releases/releases/download/v1.3.7/Retouch-1.3.7-Setup.exe)
[![macOS](https://img.shields.io/badge/macOS-purple)](https://github.com/Retouch-blog/retouch-releases/releases/download/v1.3.6/Retouch-1.3.6-arm64.dmg)
[![Discord](https://img.shields.io/discord/1528217755474591835?label=discord&logo=discord)](https://discord.gg/U63MHffDQX)
[![Website](https://img.shields.io/website?url=https%3A%2F%2Fretouch.blog&label=Website&logo=googlechrome)](https://retouch.blog)




**Retouch** est un launcher desktop qui te permet de jouer à **Dofus Touch** directement sur PC, sans émulateur Android.

Ce dépôt sert uniquement à la **distribution des builds** de Retouch — c'est ici que tu trouveras toujours la dernière version à télécharger. Site officiel : **[retouch.blog](https://retouch.blog)**

## Téléchargement (Windows)

[![Télécharger Retouch](https://img.shields.io/badge/⬇️_Cliquez_ici_pour_t%C3%A9l%C3%A9charger-Retouch--Setup.exe-2ea44f?style=for-the-badge)](https://github.com/Retouch-blog/retouch-releases/releases/download/1.3.8/Retouch-1.3.8-Setup.exe)

> ⚠️ Les exécutables ne sont pas signés (pas de certificat payant) - Windows SmartScreen peut afficher un avertissement "éditeur inconnu" au premier lancement. C'est normal pour un projet indépendant : clique sur *Informations complémentaires* → *Exécuter quand même*.

<img width="1697" height="992" alt="image" src="https://github.com/user-attachments/assets/6d33829a-2ffe-4fe7-9a67-14c228405004" />



## Téléchargement (macOS)

[![Télécharger pour Apple Silicon](https://img.shields.io/badge/⬇️_Apple_Silicon_(M1%2FM2%2FM3)-Retouch--arm64.dmg-2ea44f?style=for-the-badge)](https://github.com/Retouch-blog/retouch-releases/releases/download/v1.3.6/Retouch-1.3.6-arm64.dmg)
[![Télécharger pour Mac Intel](https://img.shields.io/badge/⬇️_Mac_Intel-Retouch--x64.dmg-2ea44f?style=for-the-badge)](https://github.com/Retouch-blog/retouch-releases/releases/download/v1.3.6/Retouch-1.3.6-x64.dmg)

> ⚠️ macOS peut bloquer l'ouverture de l'app ("développeur non identifié"), l'app n'étant pas signée avec un certificat Apple payant. Si ça arrive, ouvre le Terminal et lance cette commande :
> ```bash
> xattr -dr com.apple.quarantine "/Applications/Retouch Launcher.app"
> ```
> Relance ensuite le launcher normalement.

## Fonctionnalités

- Lance Dofus Touch dans une fenêtre desktop moderne, redimensionnable
- Toujours synchronisé avec les fichiers officiels du jeu
- Réglages de résolution (presets ou taille personnalisée), appliqués instantanément
- Interface sombre, sans bordure système, pensée pour ne pas dénaturer l'expérience de jeu
- **Multi-compte** : plusieurs comptes ouverts en simultané, chacun dans son propre onglet (barre d'onglets en haut ou sur le côté, au choix)
- **Suivi de mules (mode Héros)** : les mules suivent automatiquement le héros — changement de carte, téléportation, Zaap, et même les déplacements à l'intérieur d'une carte
- **"Courir ici"** : un clic sur la carte du monde fait voyager automatiquement le personnage jusqu'à l'endroit choisi, traversée des cartes intermédiaires comprise
- **Notifications en jeu** : message privé, invitation de groupe ou de combat remontent même depuis un onglet que tu ne regardes pas
- **Auto-accept configurable** : rejoindre / se mettre prêt automatiquement pour les invitations de combat ou de groupe sur les comptes en arrière-plan, jamais sur celui que tu contrôles activement
- **Portrait du personnage** en icône d'onglet, capturé directement depuis l'inventaire en jeu
- **Raccourcis clavier entièrement personnalisables** (sorts, interface, actions de combat...)
- **Mise à jour automatique** du launcher au démarrage — jamais besoin de retélécharger à la main


## Comment ça marche, sans zone d'ombre

Dofus Touch est en réalité un jeu HTML5/JS servi par Ankama depuis son propre CDN — pas une appli Android à émuler. Le launcher se contente de le récupérer et de l'afficher.

**01 · Téléchargement**
Le launcher récupère les fichiers du client Dofus Touch directement depuis le CDN officiel d'Ankama, comme le fait l'application mobile.

**02 · Correctifs de compatibilité**
Des correctifs de compatibilité communautaires adaptent ces fichiers pour qu'ils tournent hors du wrapper Android natif prévu par Ankama.

**03 · Service local**
Les fichiers patchés sont servis localement sur votre machine, sans jamais transiter par un serveur tiers.

**04 · Affichage natif**
Electron affiche le client dans une fenêtre desktop sur-mesure. Le jeu se re-synchronise à chaque lancement : toujours à jour, sans intervention.

## Communauté

Une question, un bug, une suggestion ? Rejoins le Discord :

💬 **[discord.gg/U63MHffDQX](https://discord.gg/U63MHffDQX)**

🌐 Site : **[retouch.blog](https://retouch.blog)**

## Avertissement

Retouch n'est pas affilié à Ankama Games, éditeur de Dofus Touch. Il fonctionne en récupérant et en adaptant des ressources du jeu pour les exécuter dans un environnement desktop non prévu à l'origine ; à ce titre, son usage peut ne pas être conforme aux conditions d'utilisation du jeu. Utilisation à tes propres risques.
