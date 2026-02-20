# Deep Dive: The Sims 2 Pets - Prima Official Game Guide

> **Source:** The Sims 2 Pets Expansion Pack - Prima Official Game Guide
> **Publisher:** Prima Games
> **Platform:** PC
> **Type:** Strategy Guide / Systems Reference

---

## Core Essence

Pets fundamentally restructures The Sims 2 household by introducing **non-player-controlled autonomous agents** that cohabit with Sims but operate under their own behavioral logic. Cats and dogs are not decorative additions -- they are full simulation entities with needs, personalities, relationships, careers, genetics, and trainable behavior. The expansion models animal cognition through a reinforcement learning framework: pets learn through praise and scolding, accumulating training points on a -100 to +100 meter that determines whether they perform or suppress 8 distinct behaviors. Wolves add a wild counterpart that can be domesticated, and werewolves inject a lycanthropic transformation system that permanently alters a Sim's personality and physique. The Pet creation system includes 108 breeds with layered genetic coat systems, and pet breeding follows Mendelian inheritance with maternal body-size weighting. Pets is the expansion that asks: what happens when you add creatures you cannot directly control to a life you can?

---

## Key Lexicon

| Term | Definition |
|------|-----------|
| **Pack Relationship** | A dog-exclusive bond (equivalent to Friend for Sims) formed when a dog reaches 50 Lifetime Relationship with a Sim/pet and has known them for 24+ hours; prevents positive relationship decay |
| **Master Relationship** | A dog-exclusive bond (equivalent to Best Friend) formed when the first Sim reaches 70 Lifetime Relationship with the dog and has known it for 24+ hours; prevents decay above Daily 25, grants passive relationship gains |
| **Mine Relationship** | A cat-exclusive bond given to any Sim/pet who reaches 60 Lifetime Relationship with the cat and has known it for 24+ hours; cats favor Mine targets and their relationship does not decay above Daily 15 |
| **Training Meter** | A -100 to +100 scale for each of 8 reinforceable behaviors; positive values mean the pet performs the behavior, negative means it suppresses it |
| **Praise / Scold** | The two reinforcement tools for training pets; each shifts the relevant behavior's training meter by a variable amount modified by Charisma skill and werewolf status |
| **Teachable Command** | One of 8 tricks (Come Here, Go Home, Play Dead, Roll Over, Shake, Sit, Speak, Stay) that can be explicitly taught to a pet via the Teach Command interaction |
| **Reinforceable Behavior** | One of 8 behavioral axes (Calm/Aggressive, Respectful/Disrespectful, Finicky/Pigpen, Housebroken/Not, Eats Pet Food/Eats Sim Food, Goes on Furniture/Stays Off, Playful/Lazy, Hostile to Strangers/Friendly) |
| **Ownership Points** | A scoring system that determines which household member a pet considers its owner; accumulated through feeding, playing, and other positive interactions |
| **Pet Career** | One of 3 career tracks (Security, Service, Showbiz) with 4 levels each; advancement requires trained commands and learned behaviors |
| **Collar** | A purchasable accessory from the Collar Connection Display at community lots; collars identify household pets and can be checked by any Sim |
| **Stray** | An unowned pet that wanders onto a lot and can be adopted via the Adopt a Stray interaction |
| **Wolf** | A wild canid that wanders lots attracted by trees, babies/toddlers, and other wolves; fixed personality (Genius, Hyper, Independent, Aggressive, Pigpen); can be domesticated at very high relationship |
| **Leader of the Pack** | A unique black wolf NPC that appears at night; source of lycanthropic infection via the Nibble interaction |
| **Savage** | A werewolf-to-Sim interaction that forcibly converts the recipient into a werewolf; accepted if recipient Mood > 0 |
| **Lycanthropic-B** | A potion ($60) purchased from the Obedience Trainer or Gypsy Matchmaker that cures werewolf infection; personality changes from infection persist after cure |
| **Obedience Trainer** | A service NPC ($25 + $75/hr) who teaches commands to pets at high-Charisma speed and sells Lycanthropic-B |
| **Kibble of Life** | An aspiration reward object with 5 charges that extends a pet's current life stage by 3 days per use; usable once per age stage |
| **Dirt Pile** | A dog-created terrain object from autonomous digging; Sims and dogs can Dig for treasures or Roll in it |
| **Diagonal Room Tool** | New build mode tool for constructing diagonally-oriented rooms |
| **Sledgehammer Tool** | New build mode deletion tool that removes objects and everything attached to them in one click |

---

## The Vibe

The Pets guide reads like a behavioral psychology manual translated into game mechanics. The training system is explicitly Skinnerian -- operant conditioning through positive and negative reinforcement, with measurable learning curves modified by the teacher's Charisma skill. Pets exist in a liminal space between controllable Sims and environmental objects: you cannot direct their actions, but you can shape their behavior over time through systematic reinforcement. The guide treats pet personalities with clinical precision, mapping 5 personality axes (Genius/Doofus, Hyper/Lazy, Independent/Friendly, Aggressive/Cowardly, Finicky/Pigpen) to behavioral probabilities. The genetics system treats coat patterns as layered alleles with dominant/recessive inheritance, and breeding outcomes follow weighted probability tables. The wolf-to-werewolf pipeline introduces a progression from wildlife encounter to supernatural transformation, with the werewolf state permanently rewriting a Sim's personality scores toward a fixed "werewolf personality" (Outgoing 10, Grouchy 0, Active 10, Sloppy 0, Playful 10). The guide's tone is pragmatic and systems-oriented, treating every pet interaction as a calculable optimization problem: which commands to teach first, how to maximize career advancement, when to breed for optimal genetic outcomes.

---

## New Mechanics Introduced

### 1. Pet Creation & Breeds
- **108 breeds:** Large dogs, small dogs, and cats each with predefined body shapes, coat patterns, and personality tendencies
- **Custom pet creation:** Full body/face customization plus coat layer system
- **Coat layers:** Base color + up to 2 overlay patterns, each with independent color, opacity, and coverage
- **5 Personality Axes:** Genius/Doofus, Hyper/Lazy, Independent/Friendly, Aggressive/Cowardly, Finicky/Pigpen
- Personality affects: autonomous behavior selection, social acceptance rates, training speed, interaction with wildlife

### 2. Pet Needs System
- **8 Needs:** Hunger, Comfort, Bladder, Energy, Fun, Social, Hygiene, and **Chew** (dogs) or **Scratch** (cats)
- Chew/Scratch are unique pet needs with no Sim equivalent -- satisfied by chewing/scratching designated objects
- Need decay rates vary by personality (Hyper pets lose Energy faster, Finicky pets lose Hygiene tolerance faster)
- Critically low Hunger triggers automatic pet removal by Animal Control (Cop NPC)

### 3. Training System (Operant Conditioning)
- **8 Reinforceable Behaviors** on individual -100 to +100 meters:
  - Calm vs. Aggressive
  - Respectful vs. Disrespectful
  - Finicky vs. Pigpen
  - Housebroken vs. Not Housebroken
  - Eats Pet Food vs. Eats Sim Food
  - Stays Off Furniture vs. Goes On Furniture
  - Playful vs. Lazy
  - Friendly to Strangers vs. Hostile to Strangers
- **Praise** shifts the meter toward the "positive" end; **Scold** shifts toward the "negative" end
- Training speed modifiers:
  - Charisma skill of the teaching Sim (+)
  - Pet's Genius trait (+) / Doofus trait (-)
  - Werewolf Sim trainer (+25% faster)
  - Obedience Trainer NPC (fastest, equivalent to high Charisma)
- Training must occur within 2 Sim-minutes of the observed behavior to register

### 4. Teachable Commands
- **8 Commands:** Come Here, Go Home, Play Dead, Roll Over, Shake, Sit, Speak, Stay
- Taught via Teach Command interaction (distinct from Praise/Scold reinforcement)
- Each command has a learning meter that fills based on repetition + teaching speed modifiers
- Fully learned commands are prerequisites for Pet Career advancement
- Commands can be performed on demand by the pet's owner

### 5. Pet Careers
- **3 Career Tracks** with **4 Levels** each:
  - **Security:** Guard Dog -> K9 -> Rescue Pet -> Pet Secret Agent
  - **Service:** Guide Dog -> Therapy Pet -> Seeing Eye Dog -> Super Hero Pet
  - **Showbiz:** Pet Extra -> Understudy -> Pet Star -> Super Star Pet
- Advancement requires: specific learned commands + specific trained behaviors + sufficient relationship with household members
- Pets leave for work via carpool and earn Simoleons
- Career performance affected by Need levels when departing

### 6. Pet Genetics & Breeding
- **Breeding:** Try for Puppy/Kitten interaction between compatible pets; 2-day gestation; litter of 1-4
- **Genome inheritance:** Each parent contributes alleles; offspring gets mix
- **Coat genetics:** Base coat layer 90% inherited from parents, overlay layers 25% inherited
- **Eye color:** Allele-based inheritance with dominant/recessive rules
- **Body size:** 70% maternal weighting (mother's body size dominates)
- Wolf + wolf = wolf offspring; wolf + dog = always dog offspring (ends wolf genetic line)
- Pet personality inherited with variation from parental averages

### 7. Pet Relationships
- **Dogs:**
  - **Pack:** Forms at 50 Lifetime + 24 hours known; no positive decay; household-only
  - **Master:** First Sim to reach 70 Lifetime + 24 hours + one more social; one Master per dog; no decay above Daily 25; passive relationship mirroring (Master's relationship gains with other Sims passively reflect onto dog)
  - Losing Master (below -80) or Master death can cause dog to run away
- **Cats:**
  - **Mine:** Forms at 60 Lifetime + 24 hours; non-exclusive (multiple Mine targets); no decay above Daily 15; cats strongly prefer interacting with Mine targets
- **All Pets:** Can have Enemies, get Furious, have Family Relationships; non-household pets can become "Pet Friend" at Daily 50+

### 8. Ownership Challenge System
- When a pet is transferred between Sims (Give Pet To, Sales Interactions), the pet's relationship to the new owner drops by Daily -10/Lifetime -10
- **Sales acceptance conditions** based on 4 possible states of Lifetime/Daily relationship combinations and Nice/Grouchy personality
- Cats may throw up after being Tossed in Air

### 9. Wildlife System
- **Skunks:** Attracted by dirty items (ash piles, dead flowers, debris, dirty diapers, puddles, trash); spray sets Hygiene to -99 and drops Fun/Comfort; 5% chance of petting success (60% for werewolves); Logic skill reduces autonomous approach probability; spray memories reduce future attempts
- **Wolves:** Attracted by trees (each 4 trees = +1% wolf visit chance), babies/toddlers, other wolves; fixed personality (Genius, Hyper, Independent, Aggressive, Pigpen); can be domesticated at very high relationship; Master requirement = Lifetime 85; Pack requirement = Lifetime 65; daily relationship decay slower (2/day vs dog's 3/day); can dig holes and knock over trash without greeting

### 10. Werewolf (Lycanthropy) System
- **Infection routes:**
  - Leader of the Pack NPC Nibble interaction (requires Lifetime/Daily 50+, Mood > 0)
  - Werewolf Sim's Savage interaction (requires target Mood > 0)
- **Transformation:** Every night at 8 PM, infected Sim transforms; reverts at 6 AM
- **Transformation effects:**
  - Hunger drops to -50 (forces immediate food seeking)
  - Energy maxes out (no sleep needed)
  - Werewolf lope (special movement animation)
  - Grr! social (Irritate interaction that frightens, causes Fun/Bladder loss)
  - Howl self-interaction (wakes sleeping Sims in room, Bladder/Comfort hit to non-werewolves, may trigger fear-based Aspiration loss)
  - Summon Wolves (outside self-interaction, attracts wolves to lot)
  - +25% pet training speed bonus
  - Excellent pet trainers (Charisma 10 equivalent)
  - Win all burglary fights (stolen items transfer to werewolf's inventory)
  - Cannot use mirrors/makeover stations
  - Can bring wolves via Summon (not Leader of the Pack)
  - Not immortal; can die in all conventional ways
  - Can stack with vampire AND zombie states simultaneously
  - Servos can become werewolves
  - Children of werewolves are normal (lycanthropy is not hereditary)
- **Slow Transformation (permanent personality drift):**
  - Outgoing -> 10 (Outgoing/Shy axis)
  - Grouchy -> 0 (Nice/Grouchy axis)
  - Active -> 10 (Active/Lazy axis)
  - Sloppy -> 0 (Neat/Sloppy axis)
  - Playful -> 10 (Playful/Serious axis)
  - Body skill drifts toward 10
  - These changes persist EVEN AFTER CURE
- **Cure:** Lycanthropic-B potion ($60 from Obedience Trainer or Gypsy Matchmaker); ends nightly transformations but personality changes remain

### 11. New Social Interactions (40+ interactions)
- **Sim-to-Pet Top Menu:** Adopt a Stray, Chase Off, Check Collar, Go to Work, Praise/Scold, Perform Command, Pick Up/Set Down, Take for a Walk (40-60 min), Teach Command, Try for Puppy/Kitten, Yell At
- **Give Love:** Feed Treat, Hug, Rub Belly, Snuggle, Stroke, Cuddle
- **Irritate:** Grr!
- **Pet-Initiated:** Ask to be Fed, Bark/Growl/Hiss (personality-based reactions from Sims), Beg for Food, Chase, Fight, Lick Toddler, Nuzzle, Ownership Challenge, Play, Pounce, Sniff
- **Play:** Cat Teaser, Fetch (with wolf), Finger Wiggle, Play With, Razzle (with wolf), Try for Puppy/Kitten (pet-to-pet)
- **Propose:** Give Pet To, Sales Interactions (with acceptance conditions based on relationship/personality)
- **Toss in Air:** Fun +50/hr for both; Energy -10/hr for Sim; cats may vomit after

### 12. New NPCs
- **Obedience Trainer:** $25 + $75/hr; teaches commands professionally; sells Lycanthropic-B ($60); marriageable (retains Charisma 10 if joined to household but loses NPC functions)
- **Cop (Animal Control):** Delivers adopted/returning pets; removes all pets if one's Hunger is critical or last teen+ Sim dies
- **Modified NPCs:** Gypsy Matchmaker now sells Lycanthropic-B; Maid cleans litter boxes, pet beds, pet houses; Mail Carrier triggers dog-specific anticipation behaviors; Gardener fills dog-dug holes

### 13. New Objects (Pet-Specific)
- Food: Good Value Pet Bowl, Scientifically Superior Pet Dish, Affluent Animal Dinner Dish (quality tiers)
- Hygiene: Mentionable Plastic Litter Box (cleanliness states affect pet willingness)
- Comfort: Comfy Pet Pillow, Pet Pillow Fantastic, Average Paws Bedding, Comfy Critter Pallet (with ownership)
- Play: Kitty Kraze Katnip, The Chewinator, Feline Birdie Stick, Scratch-O-Matic Scratching Post
- Housing: Pets' Desires House, Galactix Animal Home, Scratchpaw Manor Pet House, Los Gatos Condominiums (4-level cat condo)
- Caged Pets: FMCU 3000 womrat cage, The Basket Experience (hamster), Tropico Avian Sanctuary (bird cage with Teach to Talk)
- Business: Cat-Crazy Pet Display, Doggonit Pet Display (for Open for Business integration), Collar Connection Display

### 14. Build Mode Additions
- **Diagonal Room Tool:** Click-and-drag diagonally-oriented rooms (hotkey: Ctrl+D)
- **Diagonal Roofs:** All roof varieties except Mansard available diagonally (Long Gabled, Short Gabled, Hipped, Shed Gabled, Shed Hipped)
- **Octagonal Room Tool:** Drop and adjust octagonal rooms with keyboard resizing/rotation
- **Individual Roof Pitch Cheat:** `individualroofslopeangle [15-75]` changes individual roof slopes (Ctrl+Alt click to apply)
- **Flatten Lot Tool:** Sets entire lot elevation to match mailbox/trash can elevation
- **Sledgehammer Tool:** One-click deletion of objects and everything attached (hotkey: J); refunds depreciated value

---

## Systems & Architecture

### Training as Operant Conditioning Model
```
FOR each Reinforceable_Behavior[0..7]:
  meter: float [-100, +100]

  ON Praise(within 2 sim-minutes of behavior):
    delta = BASE_SHIFT * charisma_modifier * trait_modifier * werewolf_bonus
    meter += delta

  ON Scold(within 2 sim-minutes of behavior):
    delta = BASE_SHIFT * charisma_modifier * trait_modifier * werewolf_bonus
    meter -= delta

  Behavior_Expression:
    IF meter > 0: pet PERFORMS the positive behavior
    IF meter < 0: pet PERFORMS the negative behavior
    magnitude(meter) -> frequency/reliability of behavior
```

### Pet Career Advancement Pipeline
```
Career_Level_Requirements = {
  Security_1: [commands: {Speak}, behaviors: {Aggressive}],
  Security_2: [commands: {Speak, Stay}, behaviors: {Aggressive, Hostile}],
  ...
}

Advancement_Check:
  IF all required commands LEARNED
  AND all required behaviors TRAINED (meter > threshold)
  AND household_relationship > minimum
  THEN promote to next level
```

### Werewolf State Machine
```
State: NORMAL (6 AM - 8 PM)
  -> Sim appears human
  -> All normal interactions available
  -> Personality may be shifted from baseline

State: TRANSFORMING (8 PM trigger)
  -> Hunger = -50
  -> Energy = MAX
  -> Visual transformation to werewolf form

State: WEREWOLF (8 PM - 6 AM)
  -> Werewolf lope locomotion
  -> Grr!, Howl, Summon Wolves available
  -> +25% pet training speed
  -> Auto-win burglary fights
  -> Mirror/makeover interactions blocked
  -> Savage interaction available (infects target)

State: SLOW_DRIFT (cumulative, permanent)
  -> Each night as werewolf:
     Personality drifts toward [Out:10, Gro:0, Act:10, Slo:0, Play:10]
     Body skill drifts toward 10
  -> Changes persist even after Lycanthropic-B cure
```

### Pet Relationship Hierarchy
```
DOG relationships (in ascending order of bond strength):
  Friend (standard) -> Pack (50 LT, 24hr) -> Master (70 LT, 24hr, first Sim)

  Pack properties:
    - No positive relationship decay
    - Increased Fun/Social from interactions
    - Household-only

  Master properties:
    - No decay above Daily 25 (trends to 25 if below, not 0)
    - Passive relationship mirroring (Master gains +4 Daily with Sim B -> dog gains +2 with Sim B)
    - Enhanced Fun boost for Master when playing with dog
    - One Master per dog, sticky (requires below -80 to break)
    - Loss of Master -> possible runaway

CAT relationships:
  Friend (standard) -> Mine (60 LT, 24hr)

  Mine properties:
    - No decay above Daily 15
    - Cat strongly prefers Mine targets for autonomous interaction
    - More likely to accept socials from Mine even in bad Mood
    - Non-exclusive (cat can have multiple Mine targets)
```

### Genetics Inheritance Model
```
Offspring_Genome:
  base_coat: 90% chance inherited from random parent; 10% mutation
  overlay_1: 25% chance inherited; 75% new random
  overlay_2: 25% chance inherited; 75% new random
  eye_color: allele_system(dominant, recessive) from both parents
  body_size: 0.7 * mother.size + 0.3 * father.size
  personality: average(parent1, parent2) + random_variation

Special_Cases:
  wolf + wolf -> wolf offspring
  wolf + dog -> ALWAYS dog (wolf genetic line terminates)
  cat + cat -> cat offspring (no cross-species breeding)
```

---

## Core Insight

Pets reveals that **the most interesting simulation subjects are the ones you cannot directly control**. Every other expansion gives players new tools to direct Sim behavior -- new interactions, new aspirations, new careers. Pets introduces agents that resist direction. You cannot tell a dog to stop chewing furniture; you can only observe the behavior, intervene with reinforcement within a 2-minute window, and hope the cumulative training effect shifts the behavioral meter enough to suppress it. This is a fundamentally different design pattern: indirect control through systematic reinforcement rather than direct command. The Pack/Master/Mine relationship systems model attachment theory through game mechanics -- dogs seek hierarchical belonging (Pack = tribe, Master = alpha), while cats form possessive bonds (Mine = "I own you"). The werewolf system is the expansion's most provocative mechanic: it permanently rewrites a Sim's personality toward a fixed archetype, and even curing the condition does not undo the drift. Lycanthropy is irreversible character transformation disguised as a reversible status effect. The pet genetics system, with its maternal body-size weighting and coat layer probabilities, models biological inheritance as a predictable but non-deterministic outcome -- a fundamentally different kind of system than the precise point calculations of Chemistry or Date Scoring in Nightlife.
