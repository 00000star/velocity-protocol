# Velocity Protocol

> *Speed is the weapon.*

A Mindustry v146+ content mod focused on extreme mobility, rapid logistics, and hit-and-run tactics.

## Installation

1. **Locate** your Mindustry mods folder:
   - **Android**: `Android/data/io.anuke.mindustry/files/mods/`
   - **Desktop**: `~/.local/share/Mindustry/mods/` (Linux) or `%appdata%/Mindustry/mods/` (Windows)
   - **Steam**: Right-click Mindustry → Manage → Browse local files → `mods/`

2. **Copy** the entire `velocity-protocol` folder into the `mods/` directory.

3. **Restart** Mindustry. The mod should appear in **Settings → Mods**.

4. **Play**: Start a new map in Sandbox mode to test all units immediately.

## Content

### Units

| Unit | Type | HP | Armor | Speed | Role |
|------|------|----|-------|-------|------|
| **Runner** | Ground (Mech) | 180 | 1 | 3.2 | Ultra-fast resource hauling. No weapons. |
| **Swift** | Flying | 350 | 2 | 4.5 | Air transport. Can carry size-1 units (like Runner). |
| **Striker** | Ground (Mech) | 400 | 2 | 2.4 | Twin autocannons + Afterburner (67% speed boost near enemies). |
| **Javelin** | Hover (Flying) | 220 | 0 | 3.0 | Rail-lance artillery. Massive recoil pushes unit backward on every shot. |

### Factories

| Factory | Size | Produces | Power |
|---------|------|----------|-------|
| **Velocity Ground Factory** | 3×3 | Runner, Striker | 1.2/s |
| **Velocity Air Factory** | 3×3 | Swift, Javelin | 1.5/s |

### Special Mechanics

#### Afterburner (Striker)
When the Striker detects enemies within weapon range, a hidden system automatically engages the afterburner, applying a **67% speed boost** for 1.5 seconds (90 ticks). This enables devastating hit-and-run attacks — close in fast, unleash autocannon fire, disengage before the enemy can react.

#### Rail-Lance Recoil (Javelin)
The Javelin's rail-lance has a `recoil: 12` — roughly 4-6× the recoil of any vanilla weapon. Each shot visibly pushes the weapon mount backward. Combined with 0 armor and only 220 HP, this forces careful positional play: fire from maximum range, reposition, fire again.

## Faction Design Philosophy

The Velocity Protocol faction trades durability for speed at every level:
- **Logistics**: Runner is 3× faster than vanilla logistics units
- **Transport**: Swift can airlift ground units for instant redeployment
- **Assault**: Striker's afterburner makes it the fastest combat unit in the game
- **Artillery**: Javelin's range compensates for its paper-thin defenses

Every unit rewards aggressive micro-management and punishes static play.

## Customization

All stats are defined in plain HJSON files. To tweak balance:
- Unit stats: `content/units/*.hjson`
- Factory costs/times: `content/blocks/units/*.hjson`
- Afterburner power: `content/statuses/afterburner.hjson` → `speedMultiplier`

## Sprite Notes

The included sprites are AI-generated placeholder art. For a polished release:
1. Open sprites in [Aseprite](https://www.aseprite.org/) or [LibreSprite](https://libresprite.github.io/)
2. Redraw at the correct pixel dimensions (units: 32-48px, blocks: 96px for 3×3)
3. Match Mindustry's art style: thick outlines, flat shading, mechanical aesthetic
4. Save as 32-bit RGBA PNG

## License

MIT — Use, modify, and redistribute freely.

## Version

- **1.0.0** — Initial release with 4 units, 2 factories, 1 status effect.
