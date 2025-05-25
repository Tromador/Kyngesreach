# ⚓ Kyngesreach Naval Combat Rules  

A scalable, GURPS-compatible system for age-of-sail ship combat in
Kyngesreach, focusing on realism, tactical engagement, and historical
plausibility. 

In naval combat, the ship functions as a cohesive unit rather than a
collection of individual actions. Therefore, each vessel operates under
a unified **crew skill rating**, representing the collective competence
and training of the ship’s crew. This approach maintains simplicity and
realism by avoiding excessive tracking of individual abilities.

However, individual skill can still influence a ship’s performance.
Players and key NPCs, such as officers or veteran gunners, may leverage
their personal skills to confer advantages in critical moments. For
example, a **Leadership (Naval)** or **Tactics (Naval)** roll with a
high margin of success may accelerate gun reloading, or a decisive
action by a skilled character might sway a morale check. These
individual contributions are outlined in the relevant sections of the
rules.

This system strikes a balance between realism and playability, ensuring
that the ship remains the primary unit of action while still allowing
for heroic moments and tactical decisions by characters.  
  
This system is designed for straightforward, engaging play without the
need for detailed hex paper, miniatures, or exhaustive measurement
tools. The focus is on cinematic, narrative-driven naval combat rather
than complex tactical wargaming. Players can immerse themselves in the
action without spending the entire session on granular movement and
firing calculations. This necessarily causes some realism to be lost at
the expense of balance, compactness and speed. Some possibilities have
been fudged or even ignored completely.

## 

## 🌬️ Initiative & Position – Wind Gauge

### 📅 Round 1: Reading the Weather

Each side nominates a PC/NPC to roll ****Weather Sense****

|                          |             |
| ------------------------ | ----------- |
| **Weather Sense Result** | **Modiﬁer** |
| Success                  | \+1         |
| Critical Success         | \+2         |
| Failure                  | 0           |
| Critical Failure         | \-1         |

### 🔁 Round 2+: Contesting the Wind

Both sides roll ****Contested Seamanship**** each round.

<table>
<tbody>
<tr class="odd">
<td><strong>Modiﬁer</strong></td>
<td><strong>Eﬀect</strong></td>
</tr>
<tr class="even">
<td>Rigging hit</td>
<td>-1 per hit</td>
</tr>
<tr class="odd">
<td>Successful Tactics (Naval)</td>
<td><p>+1</p></td>
</tr>
<tr class="even">
<td>Magic Effect (eg. Trailing Wind)<sup>3</sup></td>
<td><p>+2</p></td>
</tr>
<tr class="odd">
<td><p>Handling Rating (HR) </p></td>
<td>+2 sloop/brig, +1 frigate, 0 fourth-rate, -1 ship-of-the-line </td>
</tr>
</tbody>
</table>

#### Tie Result:

  - Both sides fire **simultaneously** at **-1** accuracy.
  - Neither may switch battery.
  - Wind Gauge resets.

### 🎖️ Wind Gauge Benefits

  - Fires first
  - \+1 to Gunner (Cannon)
  - Chooses battery (port/starboard)
  - May attempt to change range

## 🧮 Firing Resolution

### 1\. Gunner (Cannon) Roll

  - Skill: Average crew 12, but can vary.
  - Apply modifiers: Wind Gauge, range, morale, damage
  - Margin of Success (MoS)¹ determines the hit rate.

### 2\. Hit Percentage

|         |              |
| ------- | ------------ |
| **MoS** | **Hit Rate** |
| 0–1     | 10%          |
| 2–3     | 25%          |
| 4–5     | 50%          |
| 6–7     | 75%          |
| 8+      | 100%         |

  - Multiply by operational guns.
  - Round down.

### 3\. Base Damage

  - The vast difference in firepower between ship classes makes it clear
    that engaging a larger opponent can be suicidal.
    
      - Sometimes the best tactic is to strike colors or attempt a
        retreat rather than face overwhelming firepower.

|                          |                       |
| ------------------------ | --------------------- |
| **Gun Calibre (in lbs)** | **Damage (Crushing)** |
| 4                        | 4d+1                  |
| 6                        | 5d-1                  |
| 9 (Sojourner)            | 6d                    |
| 12                       | 7d+1                  |
| 18                       | 8d+2                  |
| 24                       | 9d+2                  |
| 32                       | 10d+3                 |

### 4\. Penetrating Hits

  - In order to inflict significant damage, shots must penetrate hull
    armour:
    
      - As in normal combat, ship’s armour is expressed as a DR
      - Exceeding DR does Internal Damage (see below)
      - Examples as shown.

|                                   |             |
| --------------------------------- | ----------- |
| **Ship Class**                    | **Hull DR** |
| Sloop/Brig                        | 10-20       |
| Frigate (UPS Sojourner)           | 30          |
| 4<sup>th</sup> Rate               | 40          |
| 3<sup>rd</sup> Rate               | 55          |
| 2<sup>nd</sup> Rate               | 70          |
| 1<sup>st</sup> Rate (HMS Victory) | 80          |

### 5\. Reloading

  - Reloading a naval cannon takes time. 
    
      - You can’t keep all kinds of ammo to hand, hence switching takes
        longer.
      - If you have to unload before reloading, longer again

|                                      |          |
| ------------------------------------ | -------- |
| **Action**                           | **Time** |
| Reload with current ammo             | 3 rounds |
| Reload empty gun with new ammo type  | 4 rounds |
| Reload loaded gun with new ammo type | 5 rounds |

### **Reload Time Modifiers** 

  - PCs or NPCs may attempt a **Leadership (Naval)** or **Tactics
    (Naval)** check to coordinate faster reloads.

  - A **Margin of Success (MoS) of 4+** reduces **reload time by 1
    round** for the next volley.

  - **Pre-battle readiness** (e.g., powder and shot prepped) may also
    grant a **-1 round reload** bonus for the **first volley only**.
    
      - This bonus **does not stack** with other modifiers and must be
        declared in advance.

## 📏 Range Bands

  - Range modifiers reflect both the maximum possible hits and the
    difficulty of hitting at all
  - Only the ship **with the Wind Gauge** may change range.
  - On Seamanship roll: success = can shift range band by 1

|           |                  |                 |
| --------- | ---------------- | --------------- |
| **Range** | **Max Hit Rate** | **Hit Modiﬁer** |
| Extreme   | 25%              | \-4             |
| Long      | 50%              | \-2             |
| Standard  | 100%             | \+0             |
| Close     | 100%             | \+1             |

## 🚢 Internal Damage System – Hull Integrity Points (HIP)²

  - Each penetrating hull hit reduces HIP based on penetration strength
    (PS):
    
      - PS = Damage Rolled minus Ship DR
      - HIP Loss = PS to maximum of 50

|                   |                         |
| ----------------- | ----------------------- |
| **HIP Remaining** | **Status**              |
| 75–100%           | Minor damage            |
| 50–75%            | Noticeable stress       |
| 25–50%            | Severe ﬂooding          |
| 10–25%            | Critical ﬂooding        |
| 0–10%             | Rapid sinking           |
| 0                 | Ship founders and sinks |

|                     |           |
| ------------------- | --------- |
| **Ship Class**      | **HIP**   |
| Sloop/Brig          | 250       |
| Frigate (Sojourner) | 500       |
| Ship-of-the-Line    | 1000–1250 |

## 🔥 Critical Hits System (Penetrating Hull Hits)

  - ****Trigger:**** 1 crit roll per 4 penetrating hull hits in an
    attack.
  - ****Roll 1d6:**** On a 6, roll on the Critical Hit Table.

|          |                                                                |
| -------- | -------------------------------------------------------------- |
| **Roll** | **Eﬀect**                                                      |
| 1        | Fire below decks (severity scales with HIP damage).            |
| 2        | Steering damage: -1 Wind Gauge per half HIP damage.            |
| 3        | Splintering: Below deck crew casualties equal to HIP damage.   |
| 4        | Key crew injured – e.g. NCO/Officer or even a Player Character |
| 5        | Severe ﬂooding: double HIP damage.                             |
| 6        | Catastrophic hit: GM chooses dramatic eﬀect.                   |

## 🏹 Aiming & Called Shots

  - Naval cannons are not built to achieve significant elevation, making
    it exceptionally difficult to target masts and sails from the gun
    deck. 
  - The masts and visible sections of rudder present an exceptionally
    difficult target. 
  - Appropriate ammunition must be used to create damage.
  - Any ammo may be preloaded prior to combat and will be considered the
    “current” ammunition for purposes of reloading time.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Target</strong></p></td>
<td><p><strong>Ammo</strong></p></td>
<td><strong>Aiming Penalty</strong></td>
<td><strong>Range Restriction</strong></td>
<td><p><strong>DR</strong></p></td>
</tr>
<tr class="even">
<td><p>Hull</p></td>
<td><p>Round</p></td>
<td><p>0</p></td>
<td><p>Any</p></td>
<td><p>Varies</p></td>
</tr>
<tr class="odd">
<td><p>Rudder</p></td>
<td><p>Round</p></td>
<td><p>-5</p></td>
<td><p>Close</p></td>
<td><p>Hull DR -10</p></td>
</tr>
<tr class="even">
<td>Rigging/Sails</td>
<td>Chain</td>
<td>-3</td>
<td>Standard/Close</td>
<td>10</td>
</tr>
<tr class="odd">
<td><p>Masts/Spars</p></td>
<td><p>Bar</p></td>
<td><p>-6</p></td>
<td><p>Standard/Close</p></td>
<td><p>See Below</p></td>
</tr>
<tr class="even">
<td>Deck Crew</td>
<td>Grape</td>
<td>-3</td>
<td>Standard/Close</td>
<td>n/a</td>
</tr>
</tbody>
</table>

|  |
|  |
|  |

## 

## 🌲 Dismasting 

  - Each penetrating hit inflicts damage; mast collapses after 4+
    penetrating hits.
  - Research shows mast sizes aren’t that much bigger on larger ships.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Ship Class</strong></p></td>
<td><strong>Foremast DR</strong></td>
<td><strong>Mainmast DR</strong></td>
<td><strong>Mizzenmast DR</strong></td>
</tr>
<tr class="even">
<td>Sloop/Brig</td>
<td>15</td>
<td>20</td>
<td>15</td>
</tr>
<tr class="odd">
<td>Frigate (Sojourner)</td>
<td>20</td>
<td>25</td>
<td>20</td>
</tr>
<tr class="even">
<td>3<sup>rd</sup> Rate</td>
<td>25</td>
<td>30</td>
<td>25</td>
</tr>
<tr class="odd">
<td>1<sup>st</sup> Rate</td>
<td>30</td>
<td>35</td>
<td>30</td>
</tr>
</tbody>
</table>

  - Mast purposes have been much simplified, to make them distinctive.
  - 2 mast ships are considered to have a fore and main.

|               |                                                        |
| ------------- | ------------------------------------------------------ |
| **Mast Lost** | **Eﬀect**                                              |
| Foremast      | Cannot sail upwind; -2 Wind Gauge, +2 to hit for enemy |
| Mainmast      | Massive slowdown; +3 to hit for enemy                  |
| Mizzenmast    | Handling loss; -3 Wind Gauge, +1 to hit for enemy      |
| Any 2 masts   | Auto-loss of Wind Gauge; +5 to hit for enemy           |
| All masts     | Total dismasting; ship adrift. +6 to hit for enemy     |

|  |
|  |
|  |

**🌬️ Rigging & Sails Damage Effects**

  - Simple HP system to reflect gun size vs amount of sail.
  - Once damage is taken, size of ship is irrelevant. Percentage of
    ruined sails is.

|                                   |             |
| --------------------------------- | ----------- |
| **Ship Class**                    | **Sail HP** |
| Sloop/Brig                        | 100         |
| Frigate (UPS Sojourner)           | 200         |
| 4<sup>th</sup> Rate               | 300         |
| 3<sup>rd</sup> Rate               | 400         |
| 2<sup>nd</sup> Rate               | 500         |
| 1<sup>st</sup> Rate (HMS Victory) | 600         |

|                    |                 |
| ------------------ | --------------- |
| **Cannon Calibre** | **Sail Damage** |
| 9-pounder          | 10 HP           |
| 18-pounder         | 20 HP           |
| 32-pounder         | 40 HP           |

|                               |                                    |
| ----------------------------- | ---------------------------------- |
| **Sail HP Loss (% of Total)** | **Eﬀect**                          |
| 25%                           | \-1 Wind Gauge                     |
| 50%                           | \-2 Wind Gauge                     |
| 75%                           | \-4 Wind Gauge                     |
| 100%                          | Immobilised; jury rigging required |

  

🧔CREW Readiness and Crew HP System

  - Total crew complement = Crew HP (1 crew = 1 HP).
  - Max topside crew = 20% of total crew HP × current Readiness %.
  - Grape shot damage cannot exceed topside crew HP at time of impact.

|                 |                            |
| --------------- | -------------------------- |
| **Gun Calibre** | **Crew HP Damage per Hit** |
| 9-pounder       | 10                         |
| 18-pounder      | 20                         |
| 32-pounder      | 40                         |

<table>
<tbody>
<tr class="odd">
<td><p><strong>CREW</strong></p>
<p><strong>Readiness</strong></p></td>
<td><p><strong>Eﬀects</strong></p></td>
</tr>
<tr class="even">
<td>75–100%</td>
<td>No penalties.</td>
</tr>
<tr class="odd">
<td>50–75%</td>
<td>-1 Gunner, +1 reload, -1 Seamanship.</td>
</tr>
<tr class="even">
<td><p>25–50%</p></td>
<td>-2 Gunner, +2 reloads, -2 Seamanship, +1 morale check.</td>
</tr>
<tr class="odd">
<td><p>0–25%</p></td>
<td>-4 Gunner, +4 reloads, -4 Seamanship, +4 morale checks. Panic/surrender likely.</td>
</tr>
</tbody>
</table>

  - The “max topside crew” does NOT apply to a crew damage critical
    following a penetrating hit.

### 

### Footnotes

¹ Margin of Success (MoS): Difference between effective skill and roll
result.

² Hull Integrity Points (HIP): Cumulative measure of hull structural
integrity; 0 = ship sinks.

<sup>3</sup> If one side uses a magical wind spell, gain +2 Wind Gauge.

If both sides use magic, stronger effect wins; ties resolved by GM or
Quick Contest.
