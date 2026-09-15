Inventory Fix v4

This fixes the empty Whole Set Inventory issue.

Cause:
The previous special Whole Set panel was inside a JavaScript module but tried to read shopState/equipItem from a different script scope. That stopped the Whole Set inventory renderer.

Fix:
- Removed the separate Whole Set sub-panel.
- All purchased items now appear in the normal Inventory grid.
- Whole Set 01, 02, 03 show a WHOLE SET tag.
- Clicking a Whole Set equips the corresponding vrm1/vrm2/vrm3 model.
- Hoodie and Pants remain separate individual items.
