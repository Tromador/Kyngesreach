# ⚓ Kyngesreach Naval Combat Rules (WIP v1.0)

A scalable, GURPS-compatible system for age-of-sail ship combat in Kyngesreach, with a focus on realism, tactical engagement, and historical plausibility.

---

## 🌬️ Wind Gauge – Initiative & Position

### 📅 Round 1: Reading the Weather

- Each side nominates a PC/NPC to roll **Weather Sense**.
- Determines initial Wind Gauge advantage.

| Weather Sense Result | Modifier to Wind Gauge |
|----------------------|------------------------|
| Success              | +1                     |
| Critical Success     | +2                     |
| Failure              | 0                      |
| Critical Failure     | -1                     |

---

### 🔁 Round 2+: Contesting the Wind

- Both sides roll **Contested Seamanship** each round.
- Only modifiers:

| Modifier                    | Effect |
|-----------------------------|--------|
| Rigging hit                | -1 per hit |
| Successful Tactics (Naval) | +1 |
| Trailing Wind/magic        | +2 |
| Magical contest            | Quick Contest; winner applies +2 |

#### Tie Result:
- Both sides fire **simultaneously** at **-1** to accuracy.
- Neither can switch battery.
- Wind Gauge resets next round.

---

### 🎖️ Wind Gauge Benefits
- Fires first
- +1 to Gunner (Cannon)
- Chooses battery (port/starboard)
- May attempt to change range

---

## 📏 Range Bands

| Range     | Max Hit Rate | Modifier | Description |
|-----------|--------------|----------|-------------|
| Extreme   | 25%          | -4       | Ranging shots |
| Long      | 50%          | -2       | Standard engagement |
| Standard  | 100%         | +0       | Effective naval combat |
| Close     | 100%         | +1       | Grapeshot, boarding range |

- Only the ship **with Wind Gauge** may change range.
- Seamanship roll: Success = shift range by 1 band.

---

## 🧮 Firing Resolution

### 1. Gunner (Cannon) Roll
- Skill: 12 (crew average)
- Modifiers: Wind Gauge, range, morale, damage

### 2. Determine Hit Percentage

| MoS | Hit Rate |
|-----|----------|
| 0–1 | 10% |
| 2–3 | 25% |
| 4–5 | 50% |
| 6–7 | 75% |
| 8+  | 100% |

- Multiply by operational guns (default: 12 per battery).
- Round down for number of hits.

### 3. Hit Location (1d per hit)

| Roll | Location      | Effect |
|------|---------------|--------|
| 1–2  | Hull          | Roll damage vs DR |
| 3    | Rigging/Sails | -1 Wind Gauge (cumulative) |
| 4    | Deck Crew     | -10% Readiness |
| 5    | Cannons       | 1d destroyed, reload delay |
| 6    | Critical      | See revised table |

---

## 💥 Damage & Penetration Mechanics

- Assign **DR** to target ships based on class:

| Class          | DR |
|----------------|----|
| Sloop/Brig     | 10 |
| Frigate        | 20 |
| Ship of the Line| 40–50 (Victory: 50) |

- Cannon damage per calibre:
  - 9-pounder: **6d×2**
  - 18-pounder: **6d×3**
  - 32-pounder: **6d×4**

- **If damage does not exceed DR**, hit causes superficial damage only (no critical).

---

## 💥 Revised Critical Table (Penetrating Hits Only)

| Roll | Effect |
|------|--------|
| 1    | Fire on deck |
| 2    | Steering damaged |
| 3    | Magazine disruption (+1 reload round) |
| 4    | PC/NPC injury |
| 5    | Rigging collapse |
| 6    | Major hit (GM-determined severe effect, but no magic) |

- **Criticals occur only on penetrating hits**.
- **Scale with battery size** (1 critical roll per 10 guns firing, rounded up).

---

## 🚢 Sojourner's Context
- Broadside: 12 × 9-pounders per side
- Total Guns: 24
- Class: Mid-range fifth-rate frigate (~late 18th century)
- Quick, maneuverable, not designed to engage ships larger than a fourth-rate
- Effective against brigs, light frigates; outgunned by heavy frigates or ships-of-the-line

---

## 🏹 Aiming Mechanics (Planned)
To be added:
- Called shots (rigging, rudder, magazine)
- Called shot penalties
- Bonus effects for targeted hits

---

This document is a **complete snapshot** of the system to date.
