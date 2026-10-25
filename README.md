# OpenMW Controller Mods

Two separate experimental mods, each selectable through the OpenMW Data Files list after one-time native helper setup:

- **Controller Comfort 1.1:** prevents controller scroll/map zoom rollback when moving the cursor, and requires a deliberate D-pad selection before using an inventory item. Physical mouse clicks remain allowed.
- **Quick Menu Names 1.1:** adds names to all ten quick slots. A activates the selected slot, X changes its assignment, B cancels. Explicit activation can consume a potion.

See the README in each mod folder for installation, build commands, controls and limitations. Both downloadable ZIPs include corresponding source, GPL license and AI disclosure.

Quick Menu Names uses private engine interfaces. Its item-name ABI reader is restricted to executable build ID `9ae172cf58a1254ca8b63da9df7079575eeba6ab`; other portions also depend on specific native symbols. Do not assume compatibility with other builds.

## Validation scope

Controller Comfort: eight mocked inventory-guard scenarios and ten mouse/controller scroll transitions, including disabled-helper pass-through. Quick Menu Names: in-engine label layout, spell activation, cancel and assignment-dialog checks on the stated build. Real gameplay smoke tests were limited; other controllers, installations and long sessions are untested. Release builds omit the private test-only screenshot and input-injection hooks.

## AI-generated and experimental

The implementation, documentation and release packaging were generated with AI assistance through OpenAI Codex, at the author’s direction. Most code is AI-generated. Human-directed testing covers only the scenarios described here; this is not an independently audited or broadly validated release. Bugs, crashes and incompatibilities remain possible. Back up saves and configuration before trying it. No game assets or save files are distributed.

Copyright (c) 2026 kelimz. This project is licensed under GPL-3.0-only; see LICENSE. Distributed WITHOUT ANY WARRANTY. This is an unofficial project and is not endorsed by OpenMW, Bethesda, or Nexus Mods.
