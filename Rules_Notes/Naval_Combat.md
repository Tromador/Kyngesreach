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
- Margin of Success (MoS) determines the hit rate.

### 2. Hit Percentage
| MoS | Hit Rate |
|-----|----------|
| 0–1 | 10% |
| 2–3 | 25% |
| 4–5 | 50% |
| 6–7 | 75% |
| 8+  | 100% |

- Multiply by operational guns (12 per battery for Sojourner).
- Round down.

---

## 🏹 Aiming & Called Shots – Final Mechanics
| Target          | Ammo      | Aiming Penalty | Range Restriction | DR |
|-----------------|-----------|----------------|-------------------|----|
| Rudder          | Round     | -3             | Standard/Close    | Ship DR |
| Rigging/Sails   | Chain     | -3             | Standard/Close    | 10 |
| Masts/Spars     | Bar       | -6             | Standard/Close    | See below |
| Deck Crew       | Grape     | -3             | Standard/Close    | n/a |

| Ship Class        | Foremast DR | Mainmast DR | Mizzenmast DR |
|-------------------|-------------|-------------|---------------|
| Sloop/Brig        | 15          | 20          | 15            |
| Frigate (Sojourner)| 20          | 25          | 20            |
| Ship-of-the-Line  | 25          | 30          | 25            |

- Each penetrating hit inflicts damage; mast collapses after **3+ penetrating hits**.
- All aimed shots require **Standard or Close range**.

---

### 🔄 Ammunition Switching
| Action                               | Time |
|--------------------------------------|------|
| Reload with current ammo             | 3 rounds |
| Reload empty gun with new ammo type  | 4 rounds |
| Reload loaded gun with new ammo type | 5 rounds |

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
| 75%                       | -4 Wind Gauge (crippled but can still roll) |
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

## 🚢 Internal Damage System – Hull Integrity Points (HIP)

### Concept
- Each penetrating hull hit reduces **HIP** based on **penetration strength (PS)**:  
\[
PS = \text{Damage Rolled} - \text{Ship DR}
\]
- HIP loss per hit:  
\[
\text{HIP Loss} = \min(\text{PS}, 50)
\]

| Penetration Strength (PS) | HIP Loss |
|----------------------------|----------|
| 1–10                       | -10 |
| 11–20                      | -20 |
| 21–30                      | -30 |
| 31–50                      | -40 |
| >50                        | -50 |

### Revised HIP Values (scaled ×2.5)
| Ship Class        | HIP |
|-------------------|-----|
| Sloop/Brig        | 250 |
| Frigate (Sojourner)| 500 |
| Ship-of-the-Line  | 1000–1250 |

### Sinking Thresholds
| HIP Remaining | Status |
|---------------|--------|
| 75–100%      | Minor damage; cosmetic leaks |
| 50–75%       | Noticeable stress; limited system failures |
| 25–50%       | Severe flooding; impaired movement and reduced firing capability |
| 10–25%       | Critical flooding; uncontrollable flooding begins |
| 0–10%        | Rapid sinking, inevitable loss |
| 0            | Ship founders and sinks |

### Footnote
¹ **Hull Integrity Points (HIP):** A numerical measure of a ship’s overall structural integrity, representing the cumulative effect of penetrating hits to the hull. When HIP is reduced to zero, the ship founders and sinks.

---

## 🚢 Sojourner's Context
- Broadside: 12 × 9-pounders per side
- Total Guns: 24
- Class: Mid-range fifth-rate frigate (~late 18th century)
- Quick, maneuverable, but not suited for line battles against heavier ships

---

## 🧙‍♂️ Magical Wind Effects (Conditional)
- If one side uses a magical wind spell (e.g., Biele’s trailing wind), it gains **+2 Wind Gauge bonus**.  
- If both sides use magic, compare effects: stronger effect wins; if equally matched, resolve with a Quick Contest of spellcasting or GM adjudication.
