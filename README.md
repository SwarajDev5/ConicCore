# ConicDuels
**Version:** 1.5.0-DEV
**Author:** SwarajDev
**API Version:** 1.21.x
**Modrinth:** [ConicDuels on Modrinth](https://modrinth.com/plugin/conicduels)
**SpigotMC:** [ConicDuels on SpigotMC](https://www.spigotmc.org/resources/conic-duels.127583/)

ConicDuels is the core plugin for PracticePvP servers, providing **Kit**, **Party**, and **Duel** systems in one lightweight package. It includes auto-resetting arena management, stats tracking, AutoGG toggle, and is built for Paper 1.21+ with PlaceholderAPI and Hex color support.

**ConicDuels 1.5.0-DEV build is buggy & not perfectly tested, please reach out github or discord to report bugs.**
---

## 📦 Features
- Kit System (create, delete, list, give, layouts)
- Reworked Party System (create, invite, kick, fight, admin tools)
- Dedicated 1v1 Duels System with kit & rounds
- **Auto Arena Reset System** integration (Requires ConicArena + FastAsyncWorldEdit/WorldEdit)
- Arena management (create, set positions, teleport, delete, reset)
- Player stats tracking
- AutoGG toggle feature
- Fully integrated with PlaceholderAPI
- **Hex Color Code Support**
- Lightweight & optimized for performance

---

## ⌨ Commands

| Command | Aliases | Usage | Permission |
|---------|---------|-------|------------|
| `/conic` | `cc`, `coniccore` | Main admin command | `conicduels.admin` |
| `/spawn` | — | Teleport to spawn | `conicduels.spawn` |
| `/stats [player]` | `statistic`, `statistics` | View player stats | `conicduels.stats` |
| `/autoggtoggle` | — | Toggle AutoGG feature | `conicduels.autoggtoggle` |
| `/kit <create|delete|list|give|preview|rename|layouts>` | `kits`, `ck` | Kit management | `conicduels.kit` |
| `/kiteditor <edit|save|leave|reset>` | — | Edit kits privately | `conicduels.kiteditor` |
| `/arenas <create|pos1|pos2|center|list|teleport|delete|save|reset>` | — | Arena management | `conicduels.arenas.admin` |
| `/party <create|disband|invite|leave|kick|info|chat|fight|promote|demote>` | `p` | Party management | `conicduels.party` |
| `/duel <player>` | `1v1`, `battle`, `fight` | Duel another player | `conicduels.duel` |
| `/partyaccept` | — | Accept party invite | `conicduels.party` |
| `/partyfight` | — | Accept party fight | `conicduels.party` |
| `/giveeditedkit <kit> <player>` | — | Give an edited kit | `conicduels.givekit` |

---

## 🔑 Permissions

| Permission | Description | Default |
|------------|-------------|---------|
| `conicduels.*` | Access to all ConicDuels commands | `op` |
| ├─ `conicduels.admin` | Access to all admin commands (`/conic reload`, etc.) | `op` |
| ├─ `conicduels.kit` | Access to kit management commands | `true` |
| ├─ `conicduels.kiteditor` | Access to the kit editor | `true` |
| ├─ `conicduels.givekit` | Give kits to other players | `op` |
| ├─ `conicduels.arenas.admin` | Arena creation and management | `op` |
| ├─ `conicduels.party` | Access to all party commands | `true` |
| ├─ `conicduels.duel` | Access to all duel commands | `true` |
| ├─ `conicduels.spawn` | Teleport to spawn | `true` |
| ├─ `conicduels.stats` | View player stats | `true` |
| ├─ `conicduels.autoggtoggle` | Toggle AutoGG | `true` |
| ├─ `conicduels.spectate` | Spectate duels | `true` |
| ├─ `conicduels.bypass.cooldown` | Bypass all cooldowns | `op` |
| ├─ `conicduels.bypass.build` | Bypass build restrictions | `op` |
| └─ `conicduels.bypass.break` | Bypass break restrictions | `op` |

---

## ⚙ Dependencies
**Hard Dependency:**
* ConicArena

**Soft Dependencies (Required for Arena Management/Reset):**
* FastAsyncWorldEdit **or** WorldEdit

---

## 📥 Installation
1. Download the latest **ConicDuels.jar** **and** **ConicArena.jar**.
2. Place them in your server’s `/plugins` folder.
3. Ensure you also have **FastAsyncWorldEdit** or **WorldEdit** installed for arena reset functionality.
4. Start your server to generate configuration files.
5. Configure spawn and kit editing areas using:
   - `/conic setspawn`
   - `/conic setediting`
