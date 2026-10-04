# AI Packages, Alternatives & Download Links

## 1. AzzyAI (Recommended)

**Author:** Dr. Azzy (original) + community forks  

**Why use it:**
- Most actively maintained
- Excellent Homunculus S support
- GUI configuration tool
- Friend list, kiting, PvP tactics, AoE logic

### Useful Links
- Original repository: https://github.com/SpenceKonde/AzzyAI
- Kisaro fork (newer Homunculus S / 4th job skills): https://github.com/Kisaro/AzzyAI
- Other modern forks: search “AzzyAI-RE” or “AzzyAI renewal”

### Installation summary
1. Download latest release.
2. Copy contents of `USER_AI` into your client’s `AI/USER_AI/`.
3. Type `/hoai` in-game.
4. Configure with `AzzyAIConfig.exe` or by editing the `.lua` files.

---

## 2. MirAI (Legacy)

Older popular AI. Many servers still mention it, but it is largely unmaintained and can cause Lua errors on modern clients.

- Still works on some older clients.
- Has its own friend system that AzzyAI can emulate (`MirAIFriending` option).
- Not recommended for new installations in 2025+.

---

## 3. Alternative / Server-specific AIs

Many private servers ship their own modified USER_AI.  
Always prefer the version your server provides first, then fall back to AzzyAI.

Common names you may see:
- ServerName_AI
- CustomHomunAI
- AggressiveAI packs

---

## Mid-rate Specific Advice

On 10x–50x servers Homunculus level and SP regenerate faster, but monsters hit harder relative to Homunculus HP.

Recommended changes vs default AzzyAI:
- Lower `AggroHP` (start attacking earlier)
- Slightly higher skill use thresholds
- Enable `AoEMaximizeTarget` on crowded maps
- Keep `UseDanceAttack` off unless you have high SP regen

Ready-made mid-rate configs are in the `ai-config/` folder of this repository.
