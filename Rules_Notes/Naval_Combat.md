# ⚓ Kyngesreach Naval Combat Rules (v1.4 draft)

A scalable, GURPS-compatible system for age-of-sail ship combat in Kyngesreach, focusing on realism, tactical engagement, and historical plausibility.

---

## 🌬️ Wind Gauge – Initiative & Position

### 📅 Round 1: Reading the Weather
Each side nominates a PC/NPC to roll **Weather Sense**.  
| Weather Sense Result | Modifier |
|----------------------|----------|
| Success              | +1 |
| Critical Success     | +2 |
| Failure              | 0 |
| Critical Failure     | -1 |

### 🔁 Round 2+: Contesting the Wind
Both sides roll **Contested Seamanship** each round.  
| Modifier | Effect |
|----------|--------|
| Rigging hit | -1 per hit |
| Successful Tactics (Naval) | +1 |
| Trailing Wind/magic active | +2 |
| Magical contest | GM adjudication or Quick Contest |
| Handling Rating (HR) | +2 sloop/brig, +1 frigate, 0 fourth-rate, -1 ship-of-the-line |

#### Tie Result:
- Both sides fire **simultaneously** at **-1** accuracy.
- Neither may switch battery.
- Wind Gauge resets.

### 🎖️ Wind Gauge Benefits
- Fires first
- +1 to Gunner (Cannon)
- Chooses battery (port/starboard)
- May attempt to change range

---

## 📏 Range Bands
| Range     | Max Hit Rate | Modifier |
|-----------|--------------|----------|
| Extreme   | 25%          | -4 |
| Long      | 50%          | -2 |
| Standard  | 100%         | +0 |
| Close     | 100%         | +1 |

- Only the ship **with Wind Gauge** may change range.
- Seamanship roll: success = shift by 1 band.

---

## 🧮 Firing Resolution

### 1. Gunner (Cannon) Roll
- Skill: 12 (crew average)
- Apply modifiers: Wind Gauge, range, morale, damage
- Margin of Success (MoS)¹ determines the hit rate.

### 2. Hit Percentage
| MoS | Hit Rate |
|-----|----------|
| 0–1 | 10% |
| 2–3 | 25% |
| 4–5 | 50% |
| 6–7 | 75% |
| 8+  | 100% |

- Multiply by operational guns.
- Round down.

---

## 🏹 Aiming & Called Shots – Final Mechanics
| Target          | Ammo      | Aiming Penalty | Range Restriction | DR |
|-----------------|-----------|----------------|-------------------|----|
| Rudder          | Round     | -5             | Close             | Hull DR -10 |
| Rigging/Sails   | Chain     | -3             | Standard/Close    | 10 |
| Masts/Spars     | Bar       | -6             | Standard/Close    | See below |
| Deck Crew       | Grape     | -3             | Standard/Close    | n/a |

| Ship Class        | Foremast DR | Mainmast DR | Mizzenmast DR |
|-------------------|-------------|-------------|---------------|
| Sloop/Brig        | 15          | 20          | 15            |
| Frigate (Sojourner)| 20          | 25          | 20            |
| Ship-of-the-Line  | 25          | 30          | 25            |

- Each penetrating hit inflicts damage; mast collapses after 3+ penetrating hits.
- All aimed shots require Standard or Close range.

---

### 🔄 Ammunition Switching
| Action                               | Time |
|--------------------------------------|------|
| Reload with current ammo             | 3 rounds |
| Reload empty gun with new ammo type  | 4 rounds |
| Reload loaded gun with new ammo type | 5 rounds |
## 📦 Reload Time Modifiers (boxed rule)

- PCs or NPCs may attempt a **Leadership (Naval)** or **Tactics (Naval)** check to coordinate faster reloads.
- A **Margin of Success (MoS) of 4+** reduces **reload time by 1 round** for the next volley.
- **Pre-battle readiness** (e.g., powder and shot prepped) may also grant a **-1 round reload bonus for the first volley only**.
- This bonus **does not stack** with other modifiers and must be declared in advance.
---

## 🌬️ Rigging & Sails Damage – HP System
| Ship Class        | Sail HP |
|-------------------|---------|
| Sloop/Brig        | 100 |
| Frigate (Sojourner)| 200 |
| Ship-of-the-Line  | 400 |

| Cannon Calibre | Sail Damage |
|----------------|-------------|
| 9-pounder      | 10 HP |
| 18-pounder     | 20 HP |
| 32-pounder     | 40 HP |

| Sail HP Loss (% of Total) | Effect |
|---------------------------|--------|
| 25%                       | -1 Wind Gauge |
| 50%                       | -2 Wind Gauge |
| 75%                       | -4 Wind Gauge |
| 100%                      | Immobilised; jury rigging required |

---

## 🌲 Dismasting Effects
| Mast Lost    | Effect |
|--------------|--------|
| Foremast     | Cannot sail upwind; +2 to hit for enemy |
| Mainmast     | Major sail loss; +3 to hit for enemy |
| Mizzenmast   | Steering loss; +1 to hit for enemy |
| Any 2 masts  | Auto-loss of Wind Gauge; +5 to hit |
| All masts    | Total dismasting; ship adrift |

---

## 🚢 Internal Damage System – Hull Integrity Points (HIP)²

- Each penetrating hull hit reduces HIP based on penetration strength (PS):
  - PS = Damage Rolled minus Ship DR
  - HIP Loss = smaller of PS or 50

| Penetration Strength (PS) | HIP Loss |
|----------------------------|----------|
| 1–10                       | -10 |
| 11–20                      | -20 |
| 21–30                      | -30 |
| 31–50                      | -40 |
| >50                        | -50 |

| Ship Class        | HIP |
|-------------------|-----|
| Sloop/Brig        | 250 |
| Frigate (Sojourner)| 500 |
| Ship-of-the-Line  | 1000–1250 |

| HIP Remaining | Status |
|---------------|--------|
| 75–100%      | Minor damage |
| 50–75%       | Noticeable stress |
| 25–50%       | Severe flooding |
| 10–25%       | Critical flooding |
| 0–10%        | Rapid sinking |
| 0            | Ship founders and sinks |

---

## 🧑‍✈️ CREW Readiness and Crew HP System

- Total crew complement = Crew HP (1 crew = 1 HP).
- Max topside crew = 20% of total crew HP × current Readiness %.
- Grape shot damage cannot exceed topside crew HP at time of impact.

| Gun Calibre | Crew HP Damage per Hit |
|-------------|-------------------------|
| 9-pounder   | 10 |
| 18-pounder  | 20 |
| 32-pounder  | 40 |

| CREW Readiness | Effects |
|----------------|---------|
| 75–100%       | No penalties. |
| 50–75%        | -1 Gunner, +1 reload, -1 Seamanship. |
| 25–50%        | -2 Gunner, +2 reloads, -2 Seamanship, +1 morale check. |
| 0–25%         | -4 Gunner, +4 reloads, -4 Seamanship, +4 morale checks. Panic/surrender likely. |

---

## 🔥 Critical Hits System (Penetrating Hull Hits)

- **Trigger:** 1 crit roll per 4 penetrating hull hits in an attack.
- **Roll 1d6:** On a 6, roll on the Critical Hit Table.

| Roll | Effect |
|------|--------|
| 1    | Fire below decks (severity scales with HIP damage). |
| 2    | Steering damage: -1 Wind Gauge per half HIP damage. |
| 3    | Splintering: Below deck crew casualties equal to HIP damage. |
| 4    | Officer casualties: key crew injured, -10% Readiness. |
| 5    | Severe flooding: double HIP damage. |
| 6    | Catastrophic hit: GM chooses dramatic effect. |

---

### Footnotes
¹ Margin of Success (MoS): Difference between effective skill and roll result.  
² Hull Integrity Points (HIP): Cumulative measure of hull structural integrity; 0 = ship sinks.

---

## 🚢 Sojourner's Context
- Broadside: 12 × 9-pounders per side
- Total Guns: 24
- Class: Mid-range fifth-rate frigate (~late 18th century)

---

## 🧙‍♂️ Magical Wind Effects (Conditional)
- If one side uses a magical wind spell, gain +2 Wind Gauge.
- If both sides use magic, stronger effect wins; ties resolved by GM or Quick Contest.
