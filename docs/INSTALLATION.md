# Installation Guide – Full Pack

## 1. NPC & Quest Scripts

Copy these files into your server’s `npc/custom/` folder (or equivalent):

```
npc/alchemy_helper_npcs.txt
npc/genetic_trainer_npc.txt
npc/philosopher_stone_fusion.txt
npc/quest_status_npc.txt
quests/philosopher_stone_super_quest.txt
```

Then add them to your script loader (`scripts_custom.conf` or similar):

```
npc: npc/custom/alchemy_helper_npcs.txt
npc: npc/custom/genetic_trainer_npc.txt
npc: npc/custom/philosopher_stone_fusion.txt
npc: npc/custom/quest_status_npc.txt
npc: npc/custom/philosopher_stone_super_quest.txt
```

## 2. Custom Items

Add the following item IDs to your item database (or change them if they conflict):

| ID    | Name                  | Notes |
|-------|-----------------------|-------|
| 19610 | Genetic Starter Gear  | Exclusive reward |
| 19620 | Stone of the Sage     | High-tier catalyst |
| 19621 | Philosopher’s Stone   | Ultimate catalyst (very rare) |
| 19622 | Sage Fragment         | Intermediate currency |

See `docs/PHILOSOPHER_STONE_ITEMS.md` for details.

## 3. Homunculus AI (Players)

1. Install a modern AzzyAI into `AI/USER_AI/`.
2. In-game type `/hoai` until it says the Homunculus has been customized.
3. Use the mid-rate example in `ai-config/`.

## 4. Reload

```
@reloadscript
```

or restart the map server.

## Quest Flow Summary

1. Al De Baran – Brotherhood of Alchemy (start)
2. Geffen – Heart Collector (20 Immortal Hearts)
3. Lighthalzen – Biolab Courier
4. Hugel – Homunculus Resonator
5. Al De Baran – Final reward (Stone of the Sage + gear)
6. Optional: Stone of Truth Alchemist for true Philosopher’s Stone (hard)

All steps are fully scripted with proper variables and rewards.
