# ConicCore
**Version:** 1.4.0  
**Author:** SwarajDev  
**API Version:** 1.21.x  
**Modrinth:** [ConicCore on Modrinth](https://modrinth.com/plugin/conickits)  
**SpigotMC:** [ConicCore on SpigotMC](https://www.spigotmc.org/resources/conic-core.127583/)  

ConicCore is the core plugin for PracticePvP servers, providing **Kit**, **Party**, and **Duel** systems in one lightweight package. It includes arena management, stats tracking, AutoGG toggle, and is built for Paper 1.21+ with PlaceholderAPI support.
1.4.0-DEV

This is a inDev version of ConicCore, after fixing few things & adding Spawn Items, it will be officially released.
If you find some bugs, report them as soon as possible.
---

## 📦 Features
- Kit System (create, delete, list, give)
- Party System (create, invite, kick, fight)
- Duel System with kit & rounds
- Arena management (create, set positions, teleport, delete)
- Player stats tracking
- AutoGG toggle feature
- Fully integrated with PlaceholderAPI
- Lightweight & optimized for performance

---

## ⌨ Commands

| Command | Aliases | Usage | Permission |
|---------|---------|-------|------------|
| `/coniccore` | `cc`, `conic` | Main admin command | `coniccore.admin` |
| `/kit <create\|delete\|list\|give>` | `kits`, `ck` | Kit management | `coniccore.kit.*` |
| `/kiteditor <edit\|save\|leave\|reset>` | — | Edit kits privately | *(No specific node listed)* |
| `/arena <create\|pos1\|pos2\|center\|list\|teleport\|delete>` | — | Arena management | *(No specific node listed)* |
| `/party <create\|disband\|invite\|join\|leave\|kick\|info\|chat\|fight>` | `p` | Party management | `coniccore.party.*` |
| `/duel <player> <kit> <rounds>` | `1v1`, `battle`, `fight` | Duel another player | `coniccore.duel.*` |
| `/spawn` | — | Teleport to spawn | `coniccore.spawn` |
| `/stats [player]` | `statistic`, `statistics` | View player stats | `coniccore.stats` |
| `/giveeditedkit <kit> <player>` | — | Give an edited kit | *(No specific node listed)* |
| `/autoggtoggle` | — | Toggle AutoGG feature | `coniccore.autoggtoggle` |

---

## 🔑 Permissions

| Permission | Description | Default |
|------------|-------------|---------|
| `coniccore.*` | Access to all ConicCore commands | `op` |
| ├─ `coniccore.admin` | Access to all admin commands | `op` |
| ├─ `coniccore.kit.*` | Access to all kit commands | `op` |
| │ ├─ `coniccore.kit.create` | Create a kit | `op` |
| │ ├─ `coniccore.kit.delete` | Delete a kit | `op` |
| │ ├─ `coniccore.kit.list` | List all kits | `true` |
| │ └─ `coniccore.kit.give` | Give a kit to a player | `op` |
| ├─ `coniccore.party.*` | Access to all party commands | `op` |
| │ ├─ `coniccore.party.create` | Create a party | `op` |
| │ ├─ `coniccore.party.disband` | Disband a party | `op` |
| │ ├─ `coniccore.party.invite` | Invite a player to party | `op` |
| │ ├─ `coniccore.party.join` | Join a party | `op` |
| │ ├─ `coniccore.party.leave` | Leave a party | `op` |
| │ ├─ `coniccore.party.kick` | Kick a player from party | `op` |
| │ ├─ `coniccore.party.info` | Party info | `op` |
| │ ├─ `coniccore.party.chat` | Party chat | `op` |
| │ └─ `coniccore.party.fight` | Party fight | `op` |
| ├─ `coniccore.duel.*` | Access to all duel commands | `true` |
| ├─ `coniccore.spawn` | Teleport to spawn | `true` |
| ├─ `coniccore.stats` | View player stats | `true` |
| └─ `coniccore.autoggtoggle` | Toggle AutoGG | `true` |

---

## 📥 Installation
1. Download the latest `ConicCore.jar` from [Modrinth](https://modrinth.com/plugin/conickits) or [GitHub Releases](https://github.com/SwarajDev5/ConicCore/releases).
2. Place the jar into your server’s `/plugins` folder.
3. Start your server to generate configuration files.
4. Configure spawn and kit editing areas using:
