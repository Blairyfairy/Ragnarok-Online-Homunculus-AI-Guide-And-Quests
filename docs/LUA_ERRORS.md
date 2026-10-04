# Common Homunculus AI Lua Errors & Fixes

## 1. “cannot read .\AI\AI.lua” or “no such directory or file”

**Cause:** Default AI files missing or USER_AI not placed correctly.

**Fix:**
1. Make sure the folder structure is:
   ```
   RO Client/
   └── AI/
       ├── AI.lua          (official)
       ├── AI_M.lua
       └── USER_AI/        ← your custom files go here
           ├── AI.lua
           ├── H_Config.lua
           └── …
   ```
2. Re-download official default AI if the base files are missing.
3. Type `/hoai` again after fixing.

---

## 2. Continuous Lua errors after installing custom AI

**Most common causes:**
- Outdated MirAI on a modern client
- Version mismatch between AzzyAI files
- Missing `data` folder inside USER_AI
- Windows UAC blocking file writes

**Fixes:**
1. Delete the entire `USER_AI` folder.
2. Download a fresh modern AzzyAI (Kisaro or latest SpenceKonde).
3. Create an empty folder named `data` inside `USER_AI` if it does not exist.
4. Run the RO client as Administrator once (or disable UAC for the folder).
5. Type `/hoai` → Vaporize + Call.

---

## 3. “File version error” or AzzyUtil version mismatch

AzzyAI checks that all its component files are the same version.

**Fix:** Never mix files from different AzzyAI releases. Always replace the whole USER_AI set.

---

## 4. Homunculus does nothing / does not use skills

1. Confirm `/hoai` says “customized”.
2. Check `SuperPassive = False`.
3. Check `UseAttackSkill = True`.
4. Make sure Skill Class is set correctly for Homunculus S.
5. Vaporize + Call after every config change.

---

## 5. AI works then stops after relog

Some servers clear the custom AI flag.  
Just type `/hoai` again after every login.

---

## 6. Windows 10/11 specific

- Run `AzzyAIConfig.exe` as Administrator.
- Exclude the RO folder from Controlled Folder Access / antivirus.
- Avoid installing RO in `Program Files` (UAC protection).

---

If errors persist, delete USER_AI, reinstall a clean AzzyAI, and test with the most basic Aggressive settings before adding complex tactics.
