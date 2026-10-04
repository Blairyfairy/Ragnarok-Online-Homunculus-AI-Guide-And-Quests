# Installation Guide

## For Players (AI only)

1. Download a modern AzzyAI package (see [AI_PACKAGES.md](AI_PACKAGES.md)).
2. Extract into your RO client folder:
   ```
   Ragnarok Online/
   └── AI/
       └── USER_AI/          ← put all .lua files here
   ```
3. In-game type `/hoai` until the chat says **“Homunculus has been customized”**.
4. Vaporize + Call Homunculus (or relog).
5. Optionally run `AzzyAIConfig.exe` to tune settings.

## For Server GMs (full pack)

1. Copy everything under `npc/` into your `npc/custom/` folder.
2. Add the scripts to `scripts_custom.conf`.
3. Copy any custom items from the quest/NPC files into your item database.
4. Place the Super Quest NPCs on the maps listed in `docs/GENETIC_SUPER_QUEST.md`.
5. `@reloadscript`.

Mid-rate recommended rates are already written into the NPC comments and config files.
