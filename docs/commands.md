# Documentation des Commandes prises en charge par le Bot Elaxer

Dernière mise à jour : **10/11/2025**

## Introduction

Ce document liste et décrit les commandes disponibles pour le bot Discord **Elaxer**.  
Les commandes peuvent être ajoutées, modifiées ou supprimées à tout moment.  
Les permissions requises pour certaines commandes peuvent également être ajustées.

---

## Commandes Administratives

> [!IMPORTANT]
> Certaines commandes nécessitent des **permissions spécifiques**. Veuillez vérifier que vous avez les droits appropriés avant d'exécuter ces commandes.

### **Bannir un membre**
- **Permission requise** : `Administrateur` ou `Bannir des membres`
- **Commande** : `/ban {member} [reason]`
  - `{member}` (discord.User) : Membre à bannir
  - `[reason]` (str) : Raison du bannissement

### **Débannir un membre**
- **Permission requise** : `Administrateur` ou `Bannir des membres`
- **Commande** : `/unban {member} [reason]`
  - `{member}` (discord.User) : Membre à débannir
  - `[reason]` (str) : Raison du débannissement

### **Expulser un membre**
- **Permission requise** : `Administrateur` ou `Expulser des membres`
- **Commande** : `/kick {member} [reason]`
  - `{member}` (discord.User) : Membre à expulser
  - `[reason]` (str) : Raison de l'expulsion

### **Rendre muet un membre**
- **Permission requise** : `Administrateur` ou `Rendre muet un membre`
- **Commande** : `/mute {member} [duration]`
> [!WARNING]
> La commande **/mute** est actuellement en **développement**. Elle peut ne pas être fonctionnelle ou ne pas être disponible pour le moment.  
> Veuillez vérifier les mises à jour futures pour son lancement.

### **Ne plus rendre muet un membre**
- **Permission requise** : `Administrateur` ou `Rendre muet un membre`
- **Commande** : `/unmute {member}`
> [!WARNING]
> La commande **/unmute** est actuellement en **développement**. Elle peut ne pas être fonctionnelle ou ne pas être disponible pour le moment.  
> Veuillez vérifier les mises à jour futures pour son lancement.

### **Suppression de messages**
- **Permission requise** : `Administrateur` ou `Gérer les messages`
- **Commande** : `/clear {amount} [channel]`
  - `{amount}` (int) : Nombre de messages à supprimer
  - `[channel]` (discord.TextChannel) : Salon dans lequel les messages seront supprimés
> [!CAUTION]
> Utiliser la commande `/clear` peut supprimer définitivement des messages. Soyez prudent avant de l'exécuter.

### **Avertir un membre**
- **Permission requise** : `Aucune`
- **Commande** : `/warn {member} [reason]`
  - `{member}` (discord.User) : Membre à avertir
  - `[reason]` (str) : Raison de l'avertissement
> [!WARNING]
> La commande **/warn** est actuellement en **développement**. Elle peut ne pas être fonctionnelle ou ne pas être disponible pour le moment.  
> Veuillez vérifier les mises à jour futures pour son lancement.

### **Activer/Désactiver un système de Logs**
- **Commande** : `/logs {action} {id_channel}`
  - `{action}` (Literal['activate','desactivate']) : Action pour activer ou désactiver les logs
  - `{id_channel}` (str) : Salon dans lequel les logs seront affichés

### **Créer un Giveaway**
- **Commande** : `/giveaway {reward} {duree} {unite}`
  - `{reward}` (str) : Récompense du Giveaway
  - `{duree}` (int) : Durée du Giveaway
  - `{unite}` (Literal['seconde','minute','heure','jour']) : Unité de la durée
> [!WARNING]
> La commande **/giveaway** est actuellement en **développement**. Elle peut ne pas être fonctionnelle ou ne pas être disponible pour le moment.  
> Veuillez vérifier les mises à jour futures pour son lancement.

### **Obtenir un rôle via des réactions**
- **Commande** : `/reactionrole {emoji} {role_id} {message_link}`
  - `{emoji}` (str) : Emoji de la réaction
  - `{role_id}` (str) : Identifiant du rôle
  - `{message_link}` (str) : Lien du message

### **Crée un message dans un salon pour ouvrir un ticket de support**
- **Commande** : `/ticket {salon_id}`
  - `{salon_id}` (int) : Salon dans lequel sera envoyé le message pour pouvoir ouvrir un ticket
> [!WARNING]
> La commande **/ticket** est actuellement en **développement**. Elle peut ne pas être fonctionnelle ou ne pas être disponible pour le moment.  
> Veuillez vérifier les mises à jour futures pour son lancement.

---

## Commandes d'Information

### **Informations sur un membre**
- **Commande** : `/user_info {member}`
  - `{member}` (discord.Member) : Informations publiques concernant un membre

### **Informations sur un serveur**
- **Commande** : `/server_info`

---

## Commandes Fun

### **Générer un QRCode via une URL**
- **Commande** : `/qrcode {URL} [bg_color] [box_color] [box_size] [border_size]`
  - `{URL}` (str) : Lien à convertir en QRCode
  - `[bg_color]` (Literal['white','black','red','blue','green']) : Couleur du fond du QRCode
  - `[box_color]` (Literal['white','black','red','blue','green']) : Couleur du QRCode
  - `[box_size]` (int) : Taille du QRCode
  - `[border_size]` (int) : Taille de la bordure du QRCode

### **Remplacer des caractères par des caractères similaires**
- **Commande** : `/altletters {text}`
  - `{text}` (str) : Texte à transformer en caractères similaires

### ** Remplacer des caractères par le SGA**
- **Commande** : `/sga {text}`
  - `{text}` (str) : Texte à transformer en SGA

### **Une petite blague**
- **Commande** : `/blague`

### **Un petit proverbe spécial développeur**
- **Commande** : `/dev`

### **Quelques liens à propos de moi**
- **Commande** : `/alexer`

### **Jouer au puissance 4**
- **Commande** : `/puissance4 {adversaire}`
  - `{adversaire}` (discord.Member) : Adversaire de jeu

### **Jouer au pendu (SOLO)**
- **Commande** : `/pendu`

### **Jouer au pendu (AVEC UN AMI)**
- **Commande** : `/pendu_ami {adversaire}`
  - `{adversaire}` (discord.Member) : Adversaire de jeu

### **Jouer au morpion**
- **Commande** : `/morpion {adversaire}`
  - `{adversaire}` (discord.Member) : Adversaire de jeu

### **Jouer au blackjack**
- **Commande** : `/blackjack`

### **Créer un serveur entier**
- **Permission requise** : `Propriétaire du serveur`
- **Commande** : `/create_server`
> [!CAUTION]
> Utiliser la commande `/create_server` peut entièrement supprimer le serveur. Soyez prudent avant de l'exécuter.

### **Joue au Pierre-Papier-Ciseau**
- **Commande** : `/rps`

---

> [!NOTE]
> Certaines commandes nécessitent des **permissions spécifiques** pour être exécutées. Assurez-vous que vous avez les droits nécessaires avant d'utiliser ces commandes.

---

> [!TIP]  
> Pour obtenir de l’aide, poser des questions, ou discuter avec la communauté, rejoignez notre serveur Discord !
> Pour rejoindre le serveur [Discord](https://discord.gg/tz9pkUJntZ)


---

> [!NOTE]
> Si vous rencontrez un bug ou avez besoin d'aide, n'hésitez pas à m'ajouter sur discord : `.alexer`
