# Creator → Genetic Super Quest – Path of the Philosopher’s Stone

**Fully implemented multi-area quest chain.**

## Quest Variable
`PHILO_QUEST` (character variable)
- 0 = not started
- 1 = started
- 2 = hearts delivered
- 3 = sample delivered
- 4 = Homunculus resonance done
- 5 = quest complete

## Exact Steps (all scripted)

### Step 1 – Al De Baran
**NPC:** Brotherhood of Alchemy  
**Location:** `aldebaran,155,100`  
**Action:** Accept the Path → receive Acid Bottle Creation Guide  
**Sets:** `PHILO_QUEST = 1`

### Step 2 – Geffen
**NPC:** Heart Collector  
**Location:** `geffen,120,60`  
**Requirement:** 20× Immortal Heart (1037)  
**Reward:** 1× Sage Fragment  
**Sets:** `PHILO_QUEST = 2`

### Step 3 – Lighthalzen
**NPC:** Biolab Courier  
**Location:** `lighthalzen,210,310`  
**Reward:** 10 Immortal Hearts + 30 Empty Bottles + 5 Medicine Bowls  
**Sets:** `PHILO_QUEST = 3`

### Step 4 – Hugel
**NPC:** Homunculus Resonator  
**Location:** `hugel,95,145`  
**Reward:** 2× Sage Fragments  
**Sets:** `PHILO_QUEST = 4`

### Step 5 – Al De Baran (Final)
**NPC:** Brotherhood Final  
**Location:** `aldebaran,157,100`  
**Reward:**
- 1× Stone of the Sage (19620)
- 5× Sage Fragments
- 1× Exclusive Genetic/Alchemist gear (19610)
**Sets:** `PHILO_QUEST = 5`

## After the Quest
Speak with the **Stone of Truth Alchemist** (`aldebaran,140,120`) to attempt:
- Stone of the Sage creation (hard)
- True Philosopher’s Stone creation (very hard – 15% success)

## Helper NPCs
- Acid Material Trader (Al De Baran) – sells hearts, bottles, bowls, guides
- Genetic Supplier (Lighthalzen)
- Genetic Build Master (Prontera)
- Quest Chronicle (Al De Baran) – shows current step

All scripts are complete and ready to load.
