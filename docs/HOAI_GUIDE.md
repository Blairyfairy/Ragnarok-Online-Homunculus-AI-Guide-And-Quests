# Homunculus AI & `/hoai` Complete Guide

## What is `/hoai`?

`/hoai` is the client command that switches your Homunculus between the **official default AI** and the **custom USER_AI** you installed.

### How to use it

1. Summon your Homunculus.
2. Type `/hoai` in chat.
3. Look at the system message:
   - “Homunculus AI has been customized” → you are now on custom AI (AzzyAI / MirAI / etc.).
   - “Homunculus AI has been set to Basic” → you are on official AI. Type `/hoai` again.

You can switch back and forth at any time.  
After changing AI files on disk, vaporize + call (or `@refresh` if available) or relog so the new Lua is loaded.

---

## Official vs Custom AI

| Feature                    | Official AI          | Custom (AzzyAI etc.)      |
|---------------------------|----------------------|---------------------------|
| Attacks automatically     | Limited              | Fully configurable        |
| Uses skills               | Very basic           | Full skill list + tactics |
| Follows / protects owner  | Basic                | Advanced (kiting, standby)|
| Friending other players   | No                   | Yes                       |
| Homunculus S skills       | Partial              | Full support (with forks) |
| Configuration             | None                 | GUI + Lua files           |

---

## Basic Controls (while using custom AI)

- **Alt + R** → Standby / Idle mode (Homunculus stops attacking)
- **Alt + Right-click ground** → Move Homunculus to that cell
- **Alt + Double right-click monster** → Force attack that target (can trigger Berserk mode)
- Homunculus skill hotkeys still work and notify the AI

---

## Recommended First Settings (Mid-rate)

After installing AzzyAI:

1. Open `AzzyAIConfig.exe` (or edit `H_Config.lua` / `H_Tactics.lua`).
2. Homunculus tab:
   - `SuperPassive` = False
   - `AggroHP` = 30–40 (mid-rate Homunculus dies faster)
   - `UseAttackSkill` = True
3. Homunculus Tactics tab:
   - Basic Behavior = Attack (Medium) or Attack (High)
   - Skill Class = Any Skill (or Homun S Skills if you have S)
4. Apply → Vaporize + Call Homunculus.

See the `ai-config/` folder for ready-to-use mid-rate presets.
