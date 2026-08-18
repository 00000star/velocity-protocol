# Changelog

All notable changes to the Velocity Protocol mod will be documented in this file.

## [1.0.0] - 2026-08-18

### Added
- **mod.hjson**: Mod metadata (name, version, min game version 146)
- **Runner** (`content/units/runner.hjson`): Ground logistics unit, speed 3.2, HP 180, item capacity 30, no weapons
- **Swift** (`content/units/swift.hjson`): Flying transport, speed 4.5, HP 350, payload capacity 8 (carries size-1 units), no weapons
- **Striker** (`content/units/striker.hjson`): Ground assault mech, speed 2.4, HP 400, twin autocannons (18 dmg, 12 tick reload, ~24 block range), Afterburner mechanic
- **Javelin** (`content/units/javelin.hjson`): Hover artillery, speed 3.0, HP 220, rail-lance (85 dmg piercing, 90 tick reload, ~42 block range, recoil 12)
- **Afterburner** (`content/statuses/afterburner.hjson`): Custom status effect, 67% speed boost, applied automatically when Striker engages enemies
- **Velocity Ground Factory** (`content/blocks/units/velocity-ground-factory.hjson`): 3×3 factory producing Runner and Striker
- **Velocity Air Factory** (`content/blocks/units/velocity-air-factory.hjson`): 3×3 factory producing Swift and Javelin
- **Sprites**: AI-generated pixel art for all 4 units and factory block (32-bit RGBA PNG)
- **README.md**: Installation guide, content overview, mechanics documentation
