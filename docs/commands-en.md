# Documentation of Commands Supported by Elaxer Bot

Last updated: **10/11/2025**

> [!NOTE]  
> The **Elaxer** bot is currently available **in French only**.  
> A **possible future update** may include English language support.

## Introduction

This document lists and describes the commands available for the **Elaxer** Discord bot.  
Commands may be added, modified, or removed at any time.  
Permissions required for some commands may also be adjusted.

---

## Administrative Commands

> [!IMPORTANT]
> Some commands require **specific permissions**. Please ensure you have the appropriate rights before executing these commands.

### **Ban a member**
- **Permission required**: `Administrator` or `Ban Members`
- **Command**: `/ban {member} [reason]`
  - `{member}` (discord.User): Member to ban
  - `[reason]` (str): Reason for the ban

### **Unban a member**
- **Permission required**: `Administrator` or `Ban Members`
- **Command**: `/unban {member} [reason]`
  - `{member}` (discord.User): Member to unban
  - `[reason]` (str): Reason for the unban

### **Kick a member**
- **Permission required**: `Administrator` or `Kick Members`
- **Command**: `/kick {member} [reason]`
  - `{member}` (discord.User): Member to kick
  - `[reason]` (str): Reason for the kick

### **Mute a member**
- **Permission required**: `Administrator` or `Mute Members`
- **Command**: `/mute {member} [duration]`
> [!WARNING]
> The **/mute** command is currently in **development**. It may not be functional or available at the moment.  
> Please check for future updates for its release.

### **Unmute a member**
- **Permission required**: `Administrator` or `Mute Members`
- **Command**: `/unmute {member}`
> [!WARNING]
> The **/unmute** command is currently in **development**. It may not be functional or available at the moment.  
> Please check for future updates for its release.

### **Delete messages**
- **Permission required**: `Administrator` or `Manage Messages`
- **Command**: `/clear {amount} [channel]`
  - `{amount}` (int): Number of messages to delete
  - `[channel]` (discord.TextChannel): Channel where messages will be deleted
> [!CAUTION]
> Using the **/clear** command will permanently delete messages. Be careful before executing it.

### **Warn a member**
- **Permission required**: `None`
- **Command**: `/warn {member} [reason]`
  - `{member}` (discord.User): Member to warn
  - `[reason]` (str): Reason for the warning
> [!WARNING]
> The **/warn** command is currently in **development**. It may not be functional or available at the moment.  
> Please check for future updates for its release.

### **Activate/Deactivate logging system**
- **Command**: `/logs {action} {id_channel}`
  - `{action}` (Literal['activate','deactivate']): Action to activate or deactivate logs
  - `{id_channel}` (str): Channel where the logs will be shown

### **Create a Giveaway**
- **Command**: `/giveaway {reward} {duration} {unit}`
  - `{reward}` (str): Giveaway reward
  - `{duration}` (int): Giveaway duration
  - `{unit}` (Literal['second','minute','hour','day']): Unit for the duration
> [!WARNING]
> The **/giveaway** command is currently in **development**. It may not be functional or available at the moment.  
> Please check for future updates for its release.

### **Get a role via reactions**
- **Command**: `/reactionrole {emoji} {role_id} {message_link}`
  - `{emoji}` (str): Emoji for the reaction
  - `{role_id}` (str): Role ID
  - `{message_link}` (str): Message link

### **Create a message in a channel to open a support ticket**
- **Command**: `/ticket {channel_id}`
  - `{channel_id}` (int): Channel ID where the message to open a ticket will be sent
> [!WARNING]
> The **/ticket** command is currently in **development**. It may not be functional or available at the moment.  
> Please check for future updates for its release.

---

## Information Commands

### **Get information about a member**
- **Command**: `/user_info {member}`
  - `{member}` (discord.Member): Public information about a member

### **Get information about the server**
- **Command**: `/server_info`

---

## Fun Commands

### **Generate a QR Code from a URL**
- **Command**: `/qrcode {URL} [bg_color] [box_color] [box_size] [border_size]`
  - `{URL}` (str): URL to convert into a QR Code
  - `[bg_color]` (Literal['white','black','red','blue','green']): Background color of the QR Code
  - `[box_color]` (Literal['white','black','red','blue','green']): Color of the QR Code itself
  - `[box_size]` (int): Size of the QR Code
  - `[border_size]` (int): Size of the border around the QR Code

### **Replace characters with similar characters**
- **Command**: `/altletters {text}`
  - `{text}` (str): Text to transform into similar characters

### **Replace characters with SGA-style**
- **Command**: `/sga {text}`
  - `{text}` (str): Text to transform into SGA-style

### **Tell a joke**
- **Command**: `/blague`

### **Developer-specific proverb**
- **Command**: `/dev`

### **Some links about me**
- **Command**: `/alexer`

### **Play Connect Four**
- **Command**: `/puissance4 {opponent}`
  - `{opponent}` (discord.Member): Opponent to play against

### **Play Hangman (SOLO)**
- **Command**: `/pendu`

### **Play Hangman (WITH A FRIEND)**
- **Command**: `/pendu_ami {opponent}`
  - `{opponent}` (discord.Member): Opponent to play against

### **Play Tic-Tac-Toe**
- **Command**: `/morpion {opponent}`
  - `{opponent}` (discord.Member): Opponent to play against

### **Play Blackjack**
- **Command**: `/blackjack`

### **Create an entire server**
- **Permission required**: `Server Owner`
- **Command**: `/create_server`
> [!CAUTION]
> Using the **/create_server** command can completely delete the server. Be careful before executing it.

### **Play Rock-Paper-Scissors**
- **Command**: `/rps`

---

> [!NOTE]
> Some commands require **specific permissions** to be executed. Make sure you have the necessary rights before using these commands.

---

> [!TIP]  
> For help, questions, or to chat with the community, join our Discord server!  
> To join the server, click [here](https://discord.gg/tz9pkUJntZ).

---

> [!NOTE]  
> If you encounter a bug or need assistance, feel free to add me on Discord: `.alexer`
