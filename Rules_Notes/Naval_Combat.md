# ⚓ Kyngesreach Naval Combat Rules (v1.1)

A scalable, GURPS-compatible system for age-of-sail ship combat in Kyngesreach, focusing on realism, tactical engagement, and historical plausibility.

---

## 🌬️ Wind Gauge – Initiative & Position

### 📅 Round 1: Reading the Weather
- Each side nominates a PC/NPC to roll **Weather Sense**.
| Weather Sense Result | Modifier |
|----------------------|----------|
| Success              | +1 |
| Critical Success     | +2 |
| Failure              | 0 |
| Critical Failure     | -1 |

### 🔁 Round 2+: Contesting the Wind
- Both sides roll **Contested Seamanship** each round.
| Modifier                     | Effect |
|------------------------------|--------|
| Rigging hit                 | -1 per hit |
| Successful Tactics (Naval)  | +1 |
| Trailing Wind/magic active  | +2 |
| Magical contest             | GM adjudication or Quick Contest |
| Handling Rating (HR)        | +2 sloop/brig, +1 frigate, 0 fourth-rate, -1 ship-of-the-line |

#### Tie Result:
- Both sides fire **simultaneously** at **-1** to accuracy.
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

### 3. Hit Location (1d per hit)
| Roll | Location      | Effect |
|------|---------------|--------|
| 1–2  | Hull          | Damage vs DR |
| 3    | Rigging/Sails | -1 Wind Gauge (stacking) |
| 4    | Deck Crew     | -10% Readiness |
| 5    | Cannons       | 1d destroyed, reload delay |
| 6    | Critical      | See revised table |

---

## 💥 Damage & Penetration Mechanics
| Class          | DR |
|----------------|----|
| Sloop/Brig     | 10 |
| Frigate        | 20 |
| Ship of the Line| 40–50 (Victory: 50) |

| Calibre       | Damage |
|---------------|--------|
| 9-pounder     | 6d×2 |
| 18-pounder    | 6d×3 |
| 32-pounder    | 6d×4 |

- Only **penetrating hits** (damage > DR) can trigger criticals.

### Revised Critical Table
| Roll | Effect |
|------|--------|
| 1    | Fire on deck |
| 2    | Steering damaged |
| 3    | Magazine disruption |
| 4    | PC/NPC injury |
| 5    | Rigging collapse |
| 6    | Major hit (GM-determined severe effect) |

---

## 🏹 Aiming & Ammunition

### Target Areas & Required Ammo
| Target          | Ammo      | Modifier | Effect |
|-----------------|-----------|----------|--------|
| Rudder          | Round     | -2 | Steering disabled |
| Rigging/Sails   | Chain     | -2 | -1 Wind Gauge per hit; immobilise at 3+ |
| Masts/Spars     | Bar       | -3 | Mast/spar collapse |
| Deck Crew       | Grape     | -3 | -10% Readiness per hit; chance of officer injury |

- **Magazine hits are not available as called shots**; catastrophic results occur only from exceptional criticals.

---

### 🔄 Ammunition Switching – Simplified Timing
| Action                               | Time |
|--------------------------------------|------|
| Reload with current ammo             | 3 rounds |
| Reload empty gun with new ammo type  | 4 rounds |
| Reload loaded gun with new ammo type | 5 rounds |

- The powder charge remains for loaded guns; only the shot is swapped.

---

## 🚢 Sojourner's Context
- Broadside: 12 × 9-pounders per side
- Total Guns: 24
- Class: Mid-range fifth-rate frigate (~late 18th century)
- Quick, maneuverable, but not suited for line battles against heavier ships

---

## 🧙‍♂️ Magical Wind Effects (Conditional)
- Magical Wind contests (e.g., Biele vs. Stormcaller) resolved via:
  - Quick Contest of spell skills, or
  - GM adjudication if magic strength is clearly mismatched
- Applied only if both sides field magical wind-control effects.

---

This **complete snapshot** is ready for player distribution and integration into Kyngesreach sessions.
