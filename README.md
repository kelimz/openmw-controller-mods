# OpenMW Controller and Shadow Mods

AI-GENERATED AND EXPERIMENTAL. Most implementation and documentation were generated with OpenAI Codex at the author's direction. Limited local testing; no independent audit. GPL-3.0-only for our code; vendored dependencies retain their licenses. WITHOUT ANY WARRANTY.

Three separate mods, selectable in OpenMW Data Files after one-time native LD_PRELOAD setup:

- **Controller Comfort 1.1.7:** controller scroll/map rollback fixes, deliberate inventory selection, corrected Map reopening, complete dialogue-topic visibility, and persistent cursor for repeated barter +/- clicks.
- **Quick Menu Names 1.1.1:** names for ten quick slots, A Use, X Assign/change, B Cancel. This release is unchanged. Its item-name ABI reader requires executable build ID 9ae172cf58a1254ca8b63da9df7079575eeba6ab; it disables that reader on other builds.
- **Indoor Shadow Occlusion 0.2.1-experimental:** filters upper-floor actor shadows from lower floors, including open balconies. Corrects a projection synchronization bug that could hide valid nearby NPC shadows as the camera moved. Keeps indoor actor shadows enabled.

Each ZIP contains corresponding source, build scripts, installation/removal instructions and license notices. Native Linux x86-64 OpenMW 0.51.0 Flatpak extensions; see each README for exact compatibility limits. These are not Windows/macOS builds or portable Lua-only mods. Preserve all existing LD_PRELOAD helpers when installing another. No separate toggle program is required.

Controller Comfort validation includes limited in-engine Map reopening, dialogue-topic and barter-click checks. Indoor Shadow Occlusion was checked in St. Olms Waistworks at the supplied save and a nearby camera position. The saved-position NPC shadow matched native OpenMW at four sampled floor points previously suppressed by 0.2.0. Cross-floor support-plane filtering is unchanged. Other cells, renderers, controllers and long sessions remain incompletely tested.

The shadow helper uses OpenMW's directional actor shadows; it does not add shadows from lamps. Overlapping casters on different floors and irregular stairs remain limitations. Quick Menu Names relies on private engine interfaces, so other builds may lose functionality or be incompatible.

Back up saves/configuration. No game assets or save files are distributed. Copyright (c) 2026 kelimz. Unofficial; not endorsed by OpenMW, Bethesda or Nexus Mods.
