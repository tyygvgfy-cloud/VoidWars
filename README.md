# 🌌 VoidWars (BedWars) ⚔️

![Version](https://img.shields.io/badge/Version-1.0-blue)
![Platform](https://img.shields.io/badge/Platform-Spigot%20%7C%20Paper-green)
![Java](https://img.shields.io/badge/Java-8%2B-orange)

**VoidWars** is a powerful and lightweight implementation of the popular BedWars mini-game for Minecraft servers. The plugin features an advanced YAML-based interface configuration system, a full economy, and a team upgrade system.

---

## ✨ Key Features

* **📊 Dynamic Scoreboard**: Fully customize the side panel via `scoreboard.yml`. Supports colors and real-time data updates.
* **🔄 Placeholder System**:
    * `%bed_status%` — displays your bed status (✔/✘).
    * `%alive_count%` — number of surviving players in the arena.
    * `%arena_name%` — name of the current map.
* **🛒 Shop & Upgrades**: Built-in GUI menus for purchasing blocks, weapons, and armor, as well as team-wide upgrades like "Sharpness" or "Protection" using diamonds.
* **🛠 Reload Command**: Instantly refresh all configurations without restarting the server using the `/voidwars reload` command.
* **☁️ World Generator**: Automatically creates empty worlds (Void Worlds) specifically designed for arenas.

---

## 🚀 Commands & Permissions

| Command | Description | Permission |
| :--- | :--- | :--- |
| `/voidwars join <arena>` | Join a game in the specified arena | `voidwars.player` |
| `/voidwars create <name>` | Create a new arena | `voidwars.admin` |
| `/voidwars setlobby <name>` | Set the lobby point for an arena | `voidwars.admin` |
| `/voidwars reload` | Reload configs and scoreboard | `voidwars.admin` |

---

## ⚙️ Scoreboard Configuration

Example of your `scoreboard.yml`:
```yaml
scoreboard:
  title: "&b&lVOID WARS"
  lines:
    - "&7----------------"
    - "Bed status: %bed_status%"
    - "Alive players: &e%alive_count%"
    - "Arena: &f%arena_name%"
    - "&7----------------"
    - "&ewww.server.net"
