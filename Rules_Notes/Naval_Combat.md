# ⚓ Kyngesreach Naval Combat Rules (WIP v0.9)

A streamlined tactical system for handling ship-to-ship cannon engagements in the Kyngesreach campaign. Designed for GURPS but broadly compatible with narrative play.

---

## 🌬️ Wind Gauge – Initiative & Position

### 📅 Round 1: Reading the Weather

- Each side nominates a character (PC/NPC) to roll **Weather Sense**.
- This determines initial Wind Gauge advantage.

| Weather Sense Result | Modifier to Wind Gauge Contest |
|----------------------|--------------------------------|
| Success              | +1                             |
| Critical Success     | +2                             |
| Failure              | 0                              |
| Critical Failure     | -1                             |

---

### 🔁 Round 2 and Beyond: Contesting the Wind

- Each round, both ships roll a **Contested Seamanship** check.
- Only the following modifiers apply:

| Modifier                              | Effect |
|---------------------------------------|--------|
| Each rigging hit                      | -1     |
| Assisted by successful Tactics (Naval)| +1     |
| *Trailing Wind* or similar spell      | +2     |
| Magical wind contest (both sides)     | Quick Contest; winner gains +2, loser gains nothing |

#### Tie Result:
- Both ships fire **simultaneously** at **-1** to accuracy.
- **Neither** may switch batteries that round.
- No side holds Wind Gauge going into the next round.

---

### 🎖️ Wind Gauge Benefits

If your ship holds the Wind Gauge:

- **Fires first** each round
- **+1 to Gunner (Cannon)** rolls
- **Chooses which battery is facing the enemy**
- **May attempt to change range** (see below)

---

## 📏 Range Bands

Narrative positioning system with four abstract ranges.

| Range     | Max Hit Rate | Gunner (Cannon) Modifier | Description |
|-----------|--------------|--------------------------|-------------|
| Extreme   | 25%          | -2                       | Beyond standard long gun range |
| Long      | 50%          | -2                       | Cautious engagement range |
| Standard  | 100%         | +0                       | Normal broadside exchange |
| Close     | 100%         | +1                       | Grapeshot, raking fire, boarding possible |

---

### 🔁 Changing Range

- Only the ship **with Wind Gauge** may attempt to change range.
- Requires a **Seamanship** roll.

| Result            | Effect                          |
|-------------------|---------------------------------|
| Success           | Move one band closer/farther    |
| Failure           | No change                       |
| Critical Failure  | GM may rule broadside misaligns or Wind Gauge lost next round

---

## 🧮 Firing a Broadside

### 1. Gunner (Cannon) Roll
- Roll once per battery.
- Use crew skill (default: 12).
- Apply modifiers for Wind Gauge, range, damage, morale, etc.

### 2. Determine Hit Percentage

| MoS (Margin of Success) | Hit Rate |
|-------------------------|----------|
| 0–1                     | 10%      |
| 2–3                     | 25%      |
| 4–5                     | 50%      |
| 6–7                     | 75%      |
| 8+                      | 100%     |

- Multiply by the number of operational guns (default 12 per battery).
- Round down for actual number of hits.

### 3. Roll Hit Location (1d per hit)

| Roll | Location        | Effect |
|------|------------------|--------|
| 1–2  | Hull             | 6d ×2 crushing to ship HP |
| 3    | Rigging/Sails    | -1 to Wind Gauge (cumulative) |
| 4    | Deck Crew        | -10% Readiness |
| 5    | Cannons          | 1d destroyed, reload delays possible |
| 6    | Critical         | Roll on Critical Hit Table

---

## 💥 Critical Hit Table

| Roll | Effect |
|------|--------|
| 1    | **Fire on Deck** – Damage Control required |
| 2    | **Steering Damaged** – Cannot change battery; -2 Wind Gauge |
| 3    | **Magazine Rattle** – +1 round to next reload |
| 4    | **PC/NPC Injured** – Random or dramatic selection |
| 5    | **Rigging Collapse** – -3 Wind Gauge now, +1 next round if repaired |
| 6    | **Mystical Event** – Stormcaller influence, spiritual echo, or other supernatural effect

**Odds of a mystical event per hit:** 1/36 (2.78%)

---

## 🚢 Ship Crew Stat Block (Template)

Example: *Sojourner*

| Attribute         | Value  | Notes |
|------------------|--------|-------|
| Seamanship       | 12     | Used for Wind Gauge, repairs, rigging |
| Gunner (Cannon)  | 12     | Used for broadside accuracy |
| Morale           | 11     | Modified by events, PC influence, Nyxie, etc. |
| Readiness        | 100%   | Operational efficiency; affects reload and morale |
| Reload Rate      | 3 rounds | Modified by Readiness |
| Cannon Count     | 24 (12 per battery) | Track per side |

---

## 🛠 Battery Use

- Ship may fire **one battery per round** (port or starboard).
- Switching batteries requires:
  - Declaring intent
  - Spending a round to **maneuver**
  - Seamanship roll (success = battery switched next round)

- Battery may not be switched:
  - If Wind Gauge not held
  - On a tied Wind Gauge round
  - If rigging severely damaged

---

**Next Sections (in progress):**
- Readiness Loss & Recovery
- Morale System
- Damage Control Actions
- Disengagement and Chases

