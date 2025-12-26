<div align="center">

# 🧃 999Bot (User Documentation)

**External documentation for the 999Bot.** This document lists all commands that may be useful to the user.

[![Invite Bot](https://img.shields.io/badge/Discord-Invite%20Bot-7289DA?style=for-the-badge&logo=discord)](https://discord.com/oauth2/authorize?client_id=1432240754113118332)
[![Website](https://img.shields.io/badge/Website-Live%20Dashboard-FFD700?style=for-the-badge)](https://lljw.homieshouse.net/)
[![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)]()
</div>

## 🏗️ Architecture Overview

The bot operates on `discord.py` and utilizes a generic Cog system for hot-reloading.
* **Database:** `sqlite3` (Stores XP, Badges, Guild Configs, User IDs). Deletion avaliable upon request.
* **Music Source:** Direct URL streaming.
* **Hosting:** Debian  11 | 64GB RAM | AMD Ryzen 7 5800X (8C\16T)

---

## 🎵 User Commands

Available to all users in any server.

### 🔊 Music & Playback
| Command | Alias | Description | Slash Command? |
| :--- | :--- | :--- | :--- |
| `!play [song/search]` | `!p` | Plays a specific song or a random one if empty. | ✅ |
| `!search [query]` | | Searches the library and returns a selection menu. | ✅ |
| `!skip` | `!s` | Skips the current track. | ✅ |
| `!queue` | `!q` | Displays the current queue. | ✅ |
| `!addqueue [song]` | `!add` | Adds a song directly to the queue without playing immediately. | ✅ |
| `!qremove [index]` | `!qr` | Removes a specific song from the queue by its number. | ✅ |
| `!leave` | `!l` | Disconnects the bot. (Returns to camping channel if 24/7 is on). | ✅ |

### 💎 Premium Commands
| Command | Alias | Description | Slash Command? |
| :--- | :--- | :--- | :--- |
| `!file` | | DMs the user the `.mp3` file of the current song. | ❌ |
| `!247 [on/off]` | | **(Requires Server Admin)** Toggles 24/7 camping mode. | ✅ |
| `!247 [channel]` | | **(Requires Server Admin)** Sets the dedicated voice channel for the bot. | ✅ |

### 📊 Stats & Profile
| Command | Alias | Description | Slash Command? |
| :--- | :--- | :--- | :--- |
| `!badges [user]` | | View earned badges. | ❌ |
| `!leaderboard [users]` | `!lb users` | View the top 10 global users. | ❌ |
| `!leaderboard [songs]` | `!lb songs` | View the top 10 global songs. | ❌ |
| `!leaderboard` | `!lb` | Help embed for Leaderboard commands. | ❌ |
| `!help` | `!h` | Shows a help embed with all the commands. | ✅ |

---

## 👮 Administrator Commands

Requires `Administrator` permission or specific role configuration.

| Command | Alias | Description | Slash Command? |
| :--- | :--- | :--- | :--- |
| `!volume [1-100]` | | Sets the playback volume (Default: 50%). | ✅ |
| `!freestyle [on/off]` | `!fs` | Enables or Disables freestyles from the server's queue. | ✅ |
