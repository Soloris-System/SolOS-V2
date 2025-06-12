# SolOS V2 

![Python](https://img.shields.io/badge/python-3.11-blue.svg)
![discord.py](https://img.shields.io/badge/discord.py-2.3.2-7289DA.svg)
![SQLite](https://img.shields.io/badge/database-SQLite-orange.svg)
![Hosted on Replit](https://img.shields.io/badge/hosted%20on-Replit-black.svg)

**SolOS V2** is a powerful, custom-built Discord bot designed for comprehensive server management and deep community engagement. What started as a simple moderation bot has evolved into a full-fledged "Server Operating System" with a persistent database, a modular command structure, and unique features that set it apart.

---

## ✨ Key Features

*   **Persistent Database:** Powered by the built-in `sqlite3` library, all user XP, moderation logs, and role-bindings are saved permanently and survive bot restarts.
*   **XP & Leveling System:**
    *   Users earn XP passively by chatting.
    *   Custom, server-specific roles are automatically assigned based on XP milestones.
    *   A public `/leaderboard` command to foster competition.
    *   Full administrative control to add/remove XP and bind new roles.
*   **Advanced Anti-Abuse Protocol:**
    *   Monitors moderation actions (kicks/bans) from **both the bot's commands and manual Discord UI actions**.
    *   If a moderator exceeds the daily limit, their roles are automatically removed and the proper admin is alerted, preventing abuse of power.
*   **Modular Cog Architecture:** Commands are logically separated into cogs (`moderation`, `experience`, `fun`, etc.), making the code clean, organized, and easy to expand.
*   **Comprehensive Command Suite:** Over 35 commands covering everything from moderation and role management to user utilities and fun, troll-like commands.
*   **24/7 Replit Hosting:** Fully configured for deployment on Replit, including a keep-alive web server to ensure constant uptime.

---

## 🛠️ Command Modules

SolOS V2's commands are organized into the following modules:

*   **`Moderation`**: `ban`, `kick`, `audit`, `purge`, `lock`, `unlock`, `warn`, `note`, `unwarn`, `unnote`...
*   **`Experience`**: `xp`, `leaderboard`, `addxp`, `removexp`, `rbind`...
*   **`Roles`**: `role`, `unrole`, `auth`, `deauth`, `authlist`...
*   **`Fun`**: `fling`, `spammute`, `spamdeafen`...
*   **`Utility`**: `userinfo`, `serverinfo`, `poll`, `solosdmspam`, `uptime`...
*   **`Management`**: `debug`, `terminate`, `reload`, `sync`...

---

## 💻 Tech Stack

*   **Language:** Python 3.11
*   **Library:** `discord.py`
*   **Database:** `sqlite3`
*   **Hosting:** Replit
*   **Dependencies:** `pytz`, `requests`, `flask`, `waitress`

---

This project was single-handedly developed by me. Bugs will happen. Expect them.
