# Factorio 2.1 compatibility

Original prototype names and gameplay state are retained. The public mod uses its own namespace and imports the original state through native Factorio migrates_from ownership migration before legacy initialization can reset it. Test artifacts and raw player data are private.

Native Factorio 2.1.24 loaded the complete historical mod set, migrated its map and ran 600 simulation ticks. This is a headless result; it does not demonstrate a connected-client join or rendering.

The full maintained implementation is from stdlib2-continued 2.1.2 (https://github.com/goakiller900/stdlib2), retaining the legacy helper behavior under its independent public namespace. Original and continuing authors and the MIT license remain credited.

Native level-scenario assertions passed freeze/unfreeze and mining/damage protection/unprotection using current disabled_by_script and minable_flag writes.

Native userdata player/force/surface resolution and event invalidation assertions also passed.
