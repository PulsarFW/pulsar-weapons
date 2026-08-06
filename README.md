<div align="center">

<img src="https://r2.fivemanage.com/GPYOH8Hq4GPyAY7czrgLe/pulsarbanner.png" alt="Pulsar Framework" width="100%" />

<br/>

# PULSAR-WEAPONS

### Melee damage tuning and a 27-weapon custom weapon pack (models, meta, and text names)

<br/>

![Lua](https://img.shields.io/badge/Lua_5.4-2C2D72?style=flat-square&logo=lua&logoColor=white)
![FiveM](https://img.shields.io/badge/FiveM-F40552?style=flat-square)

<br/>

<sub>Enjoy the framework? A coffee helps keep active development, hardening, and support going.</sub>

<a href="https://buymeacoffee.com/pulsarframework"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 50px !important;width: 180px !important;" /></a>

<br/>

[Overview](#overview) · [Dependencies](#dependencies)

</div>

---

## Overview

Applies melee weapon damage modifiers from `GlobalState["MeleeConfig"]` via `SetWeaponDamageModifier`. Doesn't register a `plsr.X` component. General weapon handling (attachments, licensing, serials) lives in `pulsar_inventory`'s `plsr.Weapons`, not here.

Also ships a custom weapon pack under `metas/`/`stream/` — 5 melee, 1 less-lethal, 9 handguns, 2 SMGs, 6 rifles, plus reskinned taser/flashbang models. Each weapon has its own `weapons.meta`/`weaponarchetypes.meta`/`weaponanimations.meta`/`pedpersonality.meta`/`weaponcomponents.meta`, wired up via `data_file` in `fxmanifest.lua`; `client/weapon_names.lua` registers the in-game display names via `AddTextEntry`. These are native weapon definitions only — none of them have `pulsar_inventory` items yet, so they exist as usable weapon hashes but nothing currently hands them out (no `/giveweapon`-equivalent item, no shop entry). Wire that up separately if you want them obtainable in play.

---

## Dependencies

- `pulsar_core` — framework core
- `pulsar_pwnzor` — anti-cheat check loaded alongside every resource

---

## License

This resource is free to use and modify under the [Pulsar Framework License](LICENSE.md). Redistribution is welcome as long as it stays free — selling this resource or any derivative of it requires written permission from the Pulsar Framework team.

---

<div align="center">

![Pulsar Framework](https://img.shields.io/badge/Pulsar-Framework-7c3aed?style=flat-square)
![Built for FiveM](https://img.shields.io/badge/Built_for-FiveM-F40552?style=flat-square)

</div>
