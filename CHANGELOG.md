# Changes

## Controller Comfort 1.1.7
- Keep the cursor visible for repeated controller A clicks on barter price +/-.
- Includes 1.1.6: keep full D-pad-selected dialogue topics visible, including wrapped labels.
- Includes 1.1.5: remember Map through the native opening-page pass; remove the earlier delayed page switch that could flash Inventory.
- Existing time-based map zoom, scroll rollback and deliberate inventory selection fixes remain.

## Indoor Shadow Occlusion 0.2.1-experimental — new public release
- Keep native indoor actor shadows while filtering projections beyond intervening static surfaces.
- Supporting-floor planes exclude upper-floor shadows from lower floors, including open balconies.
- Synchronize blocker projection after OpenMW finalizes the shadow camera; fixes a nearby NPC shadow disappearing with camera movement.
- Linux x86-64 OpenMW Flatpak 0.51.0 f4bec41444 / OSG ABI 162 only; two shadow maps and outdoor object shadows required.

## Quick Menu Names 1.1.1 — unchanged
- Names for quick slots and A Use / X Assign / B Cancel controls.
- Private ABI item-name reader remains restricted to its documented executable build ID.

AI-generated and experimental. Source, build instructions and GPL-3.0-only license included in each ZIP. Limited local validation; see individual README files.
