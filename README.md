# 🤖 Magnum Bot — Advanced Discord Bot Showcase

<p align="center">
  <img src="https://img.shields.io/badge/Language-Go%20(Golang)-00ADD8?style=for-the-badge&logo=go" alt="Go Language">
  <img src="https://img.shields.io/badge/Database-SQLite%20(GORM)-003B57?style=for-the-badge&logo=sqlite" alt="SQLite Database">
  <img src="https://img.shields.io/badge/Status-Complete-green?style=for-the-badge" alt="Status Complete">
</p>

---

> **⚠️ NOTE: This repository serves as a showcase.**
> It contains the professional documentation and visual assets for the **Magnum Bot** project. The full source code is maintained in a private repository to protect intellectual property. This project demonstrates advanced backend architecture, concurrency management, and real-time graphics rendering using **Go**.

---

## 📖 Project Overview

Magnum Bot is a robust, modular Discord application designed for high-performance server management and engagement. It features a custom-built economy engine, a sophisticated multiplayer minigame framework, and a real-time image processing system for user profiles.

## ✨ Technical Highlights & Features

### 🖼️ Dynamic Visual Profiles
The bot features a highly advanced profile system that generates **high-quality, customized HD images** on-the-fly.
* **2D Rendering Engine:** Built natively using the `fogleman/gg` rendering library.
* **Dynamic Data Injection:** Fetches live user statistics, Discord avatars, and social links, rendering them into a custom HD buffer.
* **Custom Typography:** Implements dynamic text alignment and custom TTF font rendering.

<p align="center">
  <img src="docs/profile_showcase.png" width="90%" alt="Visual Profile Showcase" style="border-radius: 10px; border: 2px solid #333;">
  <br><em>HD Profile generated dynamically with real-time user data.</em>
</p>

---

### 💰 Economy & Casino Ecosystem
A complete, transaction-safe economy solution with a rich interactive interface.
* **Games Suite:** Includes Mines (with cashout), Lucky Jet (Crash), Blackjack, Coinflip, and **🎰 Slots (3-reel and 5-reel)**.
* **Concurrency Control:** Uses strict `sync.Mutex` locks to ensure balance integrity during high-frequency gaming sessions.

<p align="center">
  <img src="docs/casino_menu.png" width="47%" alt="Casino Main Menu">
  <img src="docs/mines_game.png" width="47%" alt="Mines Game Session">
  <br><em>Main Casino Menu and an active Mines session.</em>
</p>

<p align="center">
  <img src="docs/game_slots.png" width="47%" alt="Slots UI">
  <img src="docs/successful_spin.png" width="47%" alt="Successful Slots Win">
  <br><em>Interactive 3-reel slots and a winning spin result.</em>
</p>

---

### 🎮 Multiplayer Minigames & Scoring
A robust framework for both single-player and multiplayer sessions with a global ranking system.
* **Global Leaderboard:** A top-10 player ranking system powered by SQLite and GORM.
* **Featured Games:** * **Spy (Шпион):** Social deduction game with hidden roles distributed via DMs and case-insensitive guessing.
    * **Russian Roulette:** Features real-time drum mechanics and turn-based PvP/AI modes.
    * **Classics:** Fully interactive Tic-Tac-Toe and Hangman sessions.

<p align="center">
  <img src="docs/minigames_menu.png" width="47%" alt="Minigames Menu">
  <img src="docs/leaderboard_menu.png" width="47%" alt="Global Points Leaderboard">
  <br><em>Minigames interaction menu and the global leaderboard.</em>
</p>

---

### 🛠️ Admin & Management Suite
Powerful tools designed for administrators to manage the economy and investigate user activity.
* **Member Control:** Adjust balances, issue tools, and view detailed user stats.
* **Rig Menu (Подкрутка):** Hidden debug/admin tools to manage economy multipliers and game probabilities.

<p align="center">
  <img src="docs/admin_menu.png" width="75%" alt="Admin Member Management Panel" style="border-radius: 10px; border: 1px solid #555;">
  <br><em>Comprehensive Admin Panel for economy and member management.</em>
</p>

## 🏗️ Project Architecture

The project follows a clean, domain-driven structure to ensure maintainability:

```text
├── cmd/bot/                # Application entry point (main.go)
├── internal/
│   ├── config/             # Environment and configuration loaders
│   ├── database/           # SQLite connection and GORM Data Models
│   ├── modules/            # Core logic (Economy, Casino, Minigames)
│   └── utils/              # Helper services (Profiles, Staffmgr)
└── web/                    # Frontend assets for the web dashboard
```

## 🛠️ Tech Stack
Language: Go (Golang) — chosen for its superior concurrency primitives.

* API Wrapper: Disgo.

* Database: SQLite with GORM (Object-Relational Mapping).

* Graphics: fogleman/gg (Pure Go 2D rendering).

* Audio: Lavalink integration for high-quality streaming.

## 📬 Contact Information
* GitHub: @mchbkv

* Discord: mchbkv

* Email: mchbkv@proton.me