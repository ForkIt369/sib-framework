# THE SIMS: Complete System Architecture

> How the game works, why it works, and why 200 million people can't stop playing it.
> Synthesized from 15 books spanning the complete franchise (2000-2022).

---

## 1. THE GOD VIEW -- What You Actually Are

```
+=========================================================================+
|                                                                          |
|     You are not a player. You are a GOD.                                 |
|                                                                          |
|     But not a powerful god.                                              |
|     A god who has to remind people to pee.                               |
|                                                                          |
|     That's the joke. That's the genius. That's the game.                 |
|                                                                          |
+=========================================================================+

         +------------------+
         |    YOU (GOD)     |
         |  omniscient      |
         |  but not         |
         |  omnipotent      |
         +--------+---------+
                  |
     +------------+------------+
     |            |            |
     v            v            v
  CREATE       SUSTAIN      DIRECT
  the life     the body     the soul
  (builder)    (needs)      (goals)
     |            |            |
     v            v            v
  +------+   +--------+   +--------+
  | WHO  |   | ALIVE  |   | WHY    |
  | they |   | (keep  |   | (give  |
  | ARE  |   |  them  |   |  them  |
  |      |   |  from  |   |  mean- |
  |      |   |  dying)|   |  ing)  |
  +------+   +--------+   +--------+
```

---

## 2. THE CORE LOOP -- What Happens Every Day

```
  THE SIMS DAILY LOOP
  ====================

  +-------+     +-------+     +-------+     +-------+
  | WAKE  |---->| NEED  |---->| WANT  |---->| SLEEP |
  | UP    |     | MANAGE|     | PURSUE|     |       |
  +-------+     +-------+     +-------+     +-------+
     ^                                          |
     |                                          |
     +------ repeat until DEATH ----------------+

  EXPANDED:

  6:00 AM  +---------+
           | WAKE UP |  Energy bar refilled (if bed is good)
           +---------+
                |
                v
  6:15 AM  +---------+
           | PEE     |  Bladder bar critical from overnight
           +---------+
                |
                v
  6:30 AM  +---------+
           | SHOWER  |  Hygiene bar dropping
           +---------+
                |
                v
  7:00 AM  +---------+
           | EAT     |  Hunger bar dropping
           +---------+
                |
                v
  8:00 AM  +---------+     +---------+
           | WORK    |---->| PROMOTE |  Career track, daily tasks
           | (6 hrs) |     | or FAIL |  Skill requirements checked
           +---------+     +---------+
                |
                v
  2:00 PM  +---------+
           | SKILL   |  Build skills for next promotion
           | BUILD   |  (painting, cooking, charisma...)
           +---------+
                |
                v
  5:00 PM  +---------+
           | SOCIAL  |  Social bar dropping -- talk to someone
           | TIME    |  Build relationships for career & life
           +---------+
                |
                v
  8:00 PM  +---------+
           | FUN     |  Fun bar dropping -- watch TV, play games
           +---------+
                |
                v
  10:00 PM +---------+
           | SLEEP   |  Energy bar empty
           +---------+

  THE TRAGEDY: There are never enough hours.
  You always sacrifice something.
  That IS the game.
```

---

## 3. THE SIX NEEDS -- Gravity

```
  THE 6 NEEDS: THE GAME'S GRAVITY
  =================================
  (These bars are ALWAYS falling. You are ALWAYS fighting gravity.)

                    FULL                              EMPTY
                     |                                  |
  HUNGER     [############################............] ---> STARVATION
             eat food        cook meals     order pizza      (DEATH)

  ENERGY     [#####################...................] ---> COLLAPSE
             sleep in bed    nap on couch   coffee           (pass out
                                                              on floor)

  SOCIAL     [##############..........................] ---> ISOLATION
             talk  joke  hug  flirt  phone  chat             (depression
                                                              moodlets)

  HYGIENE    [##########################..............] ---> STENCH
             shower  bath  wash hands  brush teeth           (everyone
                                                              avoids you)

  BLADDER    [################........................] ---> ACCIDENT
             use toilet                                      (wet self,
                                                              embarrassed)

  FUN        [###########################.............] ---> BOREDOM
             TV  games  jokes  music  dance  swim            (nothing
                                                              feels good)

  THE INSIGHT:
  +-----------------------------------------------------------+
  | Every bar is a TIMER.                                      |
  | Every timer pulls you back to the BODY.                    |
  | You want to BUILD a career, LEARN piano, FALL in love --  |
  | but your Sim needs to PEE.                                 |
  |                                                            |
  | The mundane is the antagonist.                             |
  | Biology is the boss fight.                                 |
  | The toilet is the final boss.                              |
  +-----------------------------------------------------------+
```

---

## 4. THE PERSONALITY SYSTEM -- Who You Are

```
  SIMS 1: FIVE SLIDERS                    SIMS 2-4: DISCRETE TRAITS
  ========================                 =========================

  Neat    [#####-----] Sloppy             Pick 3 (permanent):
  Outgoing[########--] Shy                +----------+----------+----------+
  Active  [###-------] Lazy               | CREATIVE | ROMANTIC | GENIUS   |
  Playful [######----] Serious            +----------+----------+----------+
  Nice    [#######---] Grouchy            | EVIL     | GOOD     | LONER    |
                                          +----------+----------+----------+
  25 total points distributed             | AMBITIOUS| LAZY     | FOODIE   |
  across 5 axes.                          +----------+----------+----------+
                                          | CHEERFUL | GLOOMY   | MEAN     |
                                          +----------+----------+----------+

  EVOLUTION ACROSS ERAS:
  +------------------------------------------------------------------+
  |                                                                    |
  |  SIMS 1:  Personality = 5 sliders (analog, nuanced)              |
  |           You can be 60% Neat. Gray area exists.                  |
  |                                                                    |
  |  SIMS 2:  Personality = sliders + Aspiration + Zodiac + Turn-Ons  |
  |           Chemistry system adds ATTRACTION between Sims.          |
  |           Compatibility is computed, not just felt.               |
  |                                                                    |
  |  SIMS 3:  Personality = discrete Traits (5 chosen)               |
  |           Traits unlock unique interactions & moodlets.           |
  |           More behavioral, less statistical.                      |
  |                                                                    |
  |  SIMS 4:  Personality = 3 Traits + 1 Aspiration                  |
  |           Emotions as primary driver, not personality.            |
  |           Simplified but emotionally richer.                      |
  |                                                                    |
  +------------------------------------------------------------------+

  THE CONSTRAINT:
  +-----------------------------------------+
  | You CANNOT be Active AND Lazy.           |
  | You CANNOT be Good AND Evil.             |
  | You CANNOT be Outgoing AND Loner.        |
  |                                          |
  | Every choice closes a door.              |
  | That's what makes it YOUR Sim.           |
  +-----------------------------------------+
```

---

## 5. THE EMOTION ENGINE (Sims 4)

```
  HOW EMOTIONS WORK
  ==================

  Events generate MOODLETS (temporary emotional tokens):

  +----------+     +----------+     +----------+
  | Ate good |     | Got      |     | Saw      |
  | meal     |     | promoted |     | fire     |
  | (+Happy) |     |(+Confid) |     | (+Tense) |
  +----+-----+     +----+-----+     +----+-----+
       |                |                |
       v                v                v
  +------------------------------------------------+
  |            MOODLET STACK                        |
  |  [Happy +1] [Confident +2] [Tense +3]          |
  |                                                 |
  |  Highest stack WINS --> Dominant Emotion         |
  +------------------------+------------------------+
                           |
                           v
                    +------+-------+
                    |   TENSE      |  <-- dominant (3 > 2 > 1)
                    |  (red-orange)|
                    +--------------+
                           |
                           v
              +----------------------------+
              |  CAPABILITY GATE:           |
              |  - Cannot learn skills      |
              |  - Cannot create art        |
              |  - CAN rage-clean           |
              |  - CAN confront enemies     |
              +----------------------------+

  THE 15 EMOTIONS AS CAPABILITY GATES:

  HAPPY -----> amplifies everything           (GREEN)
  FOCUSED ---> skill learning x2              (TEAL)
  INSPIRED --> creative output unlocked       (CYAN)
  CONFIDENT -> social success boosted         (YELLOW)
  ENERGIZED -> exercise/work enhanced         (LIME)
  FLIRTY ----> romantic actions unlocked      (PINK)
  PLAYFUL ---> humor/fun actions boosted      (ORANGE)

  ANGRY -----> blocks learning, enables rage  (RED)
  SAD -------> blocks most actions            (BLUE)
  TENSE -----> blocks creativity              (RED-ORANGE)
  EMBARRASSED> trust penalty                  (PURPLE)
  BORED -----> engagement drops               (GRAY)
  UNCOMFORTABLE> blocks activities            (BROWN)
  DAZED -----> nearly useless                 (STARS)

  FINE ------> neutral baseline               (no color)

  KEY INSIGHT:
  Emotions are NOT cosmetic. They are FUNCTIONAL.
  An angry Sim literally CANNOT learn.
  A tense Sim literally CANNOT create.
  Your emotional state determines what is POSSIBLE.
```

---

## 6. THE CAREER LADDER

```
  HOW CAREERS WORK
  =================

  Level 1          Level 5            Level 10
  (entry)          (FORK)             (mastery)
    |                |                    |
    v                v                    v
  +------+     +----+----+          +--------+
  |$100  |     | CHOOSE  |     A:   |$2,000  |
  |/day  |---->| A or B  |----+---->|/day    |
  |      |     |         |    |     |        |
  |no    |     |skills   |    |     |max     |
  |skills|     |required |    |     |skills  |
  +------+     +---------+    |     +--------+
                              |
                              |     +--------+
                              +---->|$1,800  |  B:
                                    |/day +  |
                                    |royalty |
                                    +--------+

  THE 8 CAREER TRACKS (Sims 4):

  ASTRONAUT --------+-- Space Ranger ($11,816/wk)
                    +-- Interstellar Smuggler ($14,868/wk)

  TECH GURU ---------+-- E-Sport Gamer ($7,872/wk)
                     +-- Start-Up Entrepreneur ($7,740/wk + royalties)

  CRIMINAL ----------+-- Boss ($12,460/wk)
                     +-- Oracle/Hacker ($8,848/wk)

  WRITER ------------+-- Author ($5,580/wk + royalties)
                     +-- Journalist ($6,888/wk)

  PAINTER -----------+-- Master of the Real ($4,920/wk + sales)
                     +-- Patron of the Arts ($6,560/wk)

  SECRET AGENT ------+-- Diamond Agent ($12,780/wk)
                     +-- Villain ($12,875/wk)

  ENTERTAINMENT -----+-- Musician ($9,520/wk)
                     +-- Comedian ($8,532/wk)

  CULINARY ----------+-- Chef ($9,840/wk)
                     +-- Mixologist ($5,910/wk)

  WHAT PROMOTIONS REQUIRE:
  +------------------------------------------+
  | Skill Level (e.g., Logic 5)              |
  | + Relationship (e.g., 2 friends)         |
  | + Daily Task (e.g., "practice speech")   |
  | + Mood (e.g., arrive Confident)          |
  +------------------------------------------+

  THE GUIDE'S OBSESSION: $/week per career.
  The "best" career is the one that pays most
  for least time. Crime literally pays.
```

---

## 7. THE SKILL TREE

```
  20 SKILLS, EACH LEVEL 1-10
  ============================

  Every skill unlocks new ACTIONS at each level:

  Level:  1     2     3     4     5     6     7     8     9    10
          |     |     |     |     |     |     |     |     |     |
          v     v     v     v     v     v     v     v     v     v
  COOKING [.][..][...][....][.....][......][.......][........][.........][..........]
          |                       |                                      |
          v                       v                                      v
       make salad           make lobster                          AMBROSIA
       (bad quality)        (good quality)                    (resurrects dead)

  SKILLS MAP:
  +------------------+--------------------+------------------------+
  | CATEGORY         | SKILLS             | WHAT THEY UNLOCK       |
  +------------------+--------------------+------------------------+
  | Creative         | Painting           | Sell art, emotional    |
  |                  | Writing            | Publish books, royalty |
  |                  | Guitar/Piano/Violin| Perform, tip jar       |
  |                  | Comedy             | Open mic, entertain    |
  +------------------+--------------------+------------------------+
  | Mental           | Logic              | Chess, career req      |
  |                  | Programming        | Games, hacking, apps   |
  |                  | Rocket Science     | Build/fly rockets      |
  |                  | Handiness          | Fix/upgrade objects    |
  +------------------+--------------------+------------------------+
  | Physical         | Fitness            | Gym, stamina, fight    |
  |                  | Cooking            | Feed household         |
  |                  | Gourmet Cooking    | Fine dining            |
  |                  | Mixology           | Cocktails, bartend     |
  +------------------+--------------------+------------------------+
  | Social           | Charisma           | Persuade, career req   |
  |                  | Mischief           | Troll, prank, deceive  |
  +------------------+--------------------+------------------------+
  | Outdoor          | Gardening          | Grow food, rare plants |
  |                  | Fishing            | Catch food, rare fish  |
  +------------------+--------------------+------------------------+
  | Gaming           | Video Gaming       | Compete, stream, earn  |
  +------------------+--------------------+------------------------+

  THE SIDE HUSTLE ECONOMY:
  Skills = money printers that don't require a job.
  A painter makes $1000+ per masterpiece.
  A writer earns royalties while sleeping.
  A programmer creates games that generate passive income.
```

---

## 8. THE RELATIONSHIP WEB

```
  HOW RELATIONSHIPS WORK
  =======================

  Every relationship has TWO independent bars:

       FRIENDSHIP (green)                ROMANCE (pink)
       -100          0         +100      -100         0         +100
        |            |           |        |           |           |
  [ENEMY]     [STRANGER]    [BFF]   [none]     [crush]     [SOULMATE]

  BUILT THROUGH:                    BUILT THROUGH:
  - Talk, Joke, Compliment          - Flirt, Kiss, WooHoo
  - Help, Share, Gift               - Romantic dinner, Stars
  - Negative: Insult, Fight         - Negative: Cheat, Reject

  THE SOCIAL ACTIONS TREE:

  FRIENDLY -----> Talk / Joke / Compliment / Hug / Cheer Up
       |
  MISCHIEF -----> Troll / Prank / Deceive / Insult
       |
  ROMANTIC -----> Flirt / Kiss / Embrace / Propose / WooHoo
       |
  MEAN ---------> Argue / Fight / Mock / Betray

  RELATIONSHIP MILESTONES:
  +------------------+-------------------------------------------+
  | Acquaintance     | Met once, name known                      |
  | Friend           | Friendship bar > 50                       |
  | Good Friend      | Friendship bar > 60                       |
  | Best Friend (BFF)| Friendship bar > 80 + "BFF" interaction   |
  | Crush            | Romance bar > 30                          |
  | Boyfriend/GF     | "Ask to be" interaction accepted          |
  | Fiance           | Proposal accepted                         |
  | Spouse           | Wedding ceremony                          |
  | Enemy            | Friendship bar < -50                      |
  +------------------+-------------------------------------------+

  WHY RELATIONSHIPS MATTER:
  +--------------------------------------------------+
  | Careers REQUIRE friends for promotion.            |
  | (e.g., "Have 3 friends" to reach Level 7)        |
  |                                                   |
  | Marriage = permanent Social need battery.          |
  | (Always someone to talk to at home)               |
  |                                                   |
  | Children = legacy vehicles.                       |
  | (Next generation inherits the house and wealth)   |
  |                                                   |
  | Every relationship is a RESOURCE.                 |
  | That's the game's coldest truth.                  |
  +--------------------------------------------------+
```

---

## 9. THE HOUSE -- Your Physical Universe

```
  BUILD MODE: WHERE CREATIVITY LIVES
  ====================================

  +--[ LOT ]-----------------------------------------------+
  |                                                         |
  |   +--[ HOUSE ]--------------------------------------+  |
  |   |                                                  |  |
  |   |        /\                                        |  |
  |   |       /  \  ROOF (style, color, pitch)           |  |
  |   |      /    \                                      |  |
  |   |     /------\                                     |  |
  |   |    |        |                                    |  |
  |   |    | FLOOR 2|  (OPTIONAL - stairs waste time!)   |  |
  |   |    |        |                                    |  |
  |   |    |--------|                                    |  |
  |   |    |  BED   |  BATH  |  KID'S  |                 |  |
  |   |    |  ROOM  |  ROOM  |  ROOM   |                 |  |
  |   |    |--------|--------|---------|                 |  |
  |   |    | LIVING ROOM     | KITCHEN |                 |  |
  |   |    |  (TV, couch,    | (stove, |                 |  |
  |   |    |   bookcase)     |  fridge)|                 |  |
  |   |    |-----------------|---------|                 |  |
  |   |    [    FOUNDATION             ]                 |  |
  |   +--------------------------------------------------+  |
  |                                                         |
  |   === YARD ===                                          |
  |   [garden] [grill] [pool] [mailbox] [trash]             |
  |                                                         |
  +---------------------------------------------------------+

  OBJECT QUALITY TIERS:
  +--------+----------+-----------+
  | CHEAP  | MID-TIER | EXPENSIVE |
  | $200   | $800     | $3,000   |
  | breaks | works    | BOOSTS   |
  | often  | fine     | NEEDS    |
  +--------+----------+-----------+
      |         |           |
      v         v           v
  bad mood   neutral    +2 Fun
  fires      reliable   +3 Comfort
  stink      adequate   faster skill

  THE GUIDE'S #1 BUILDING RULE:
  +-----------------------------------------------+
  | DON'T BUILD BIG.                               |
  |                                                 |
  | Walking from room to room WASTES TIME.          |
  | Stairs WASTE TIME.                              |
  | Long hallways WASTE TIME.                       |
  |                                                 |
  | The optimal house is SMALL and EFFICIENT:       |
  | - Bed near bathroom (wake -> pee -> shower)     |
  | - Kitchen near dining (cook -> eat)             |
  | - Skill objects near each other                 |
  | - NO second floor unless you're rich            |
  |                                                 |
  | FUNCTIONALITY > AESTHETICS. ALWAYS.             |
  +-----------------------------------------------+
```

---

## 10. THE EXPANSION LAYER CAKE -- How The Franchise Grew

```
  EACH EXPANSION ADDS A NEW DIMENSION TO LIFE
  =============================================

  SIMS 4 (2014)     BASE: Needs + Emotions + Skills + Careers + Relationships
  ─────────────────────────────────────────────────────────────────────────────
  SIMS 3 (2009-2012)
  ─────────────────────────────────────────────────────────────────────────────
  |  WORLD           | AMBITIONS        | LATE NIGHT       | SHOWTIME        |
  |  ADVENTURES      |                  |                  |                 |
  |  +travel         | +active careers  | +celebrity       | +performance    |
  |  +tombs          | +self-employment | +fame/scandal    | +stage careers  |
  |  +martial arts   | +firefighter     | +vampires        | +singer         |
  |  +nectar making  | +investigator    | +nightclubs/bars | +magician       |
  |  +visa levels    | +ghost hunter    | +bands           | +acrobat        |
  |  +China/France/  | +sculpting       | +mixology        | +SimFest        |
  |   Egypt          | +inventing       | +hot spots       | +SimPort        |
  |                  | +tattooing       | +penthouse       | +feat queue     |
  ─────────────────────────────────────────────────────────────────────────────
  SIMS 2 (2004-2008)
  ─────────────────────────────────────────────────────────────────────────────
  |  NIGHTLIFE       | PETS             | SEASONS          |                 |
  |  +dating system  | +cats & dogs     | +weather         |                 |
  |  +chemistry      | +operant cond.   | +temperature     |                 |
  |  +restaurants    | +pet careers     | +gardening       |                 |
  |  +vampires       | +108 breeds      | +PlantSims       |                 |
  |  +downtown       | +werewolves      | +fishing         |                 |
  |  +fury system    | +pack bonds      | +seasonal acts   |                 |
  |                  |                  |                  |                 |
  |  BON VOYAGE      | FREE TIME        | APARTMENT LIFE   |                 |
  |  +vacations      | +hobbies (10)    | +shared lots     |                 |
  |  +3 destinations | +enthusiasm      | +landlords       |                 |
  |  +mementos       | +The Zone        | +witchcraft      |                 |
  |  +secret lots    | +crafting        | +social class    |                 |
  |  +Bigfoot        | +BFF system      | +reputation      |                 |
  |  +voodoo doll    | +study topics    | +social groups   |                 |
  ─────────────────────────────────────────────────────────────────────────────
  SIMS 1 (2000-2003)
  ─────────────────────────────────────────────────────────────────────────────
  |  BASE GAME       | LIVIN' LARGE     | HOUSE PARTY      | BUSTIN' OUT     |
  |  +5 personality  | +new careers     | +party system     | +goal-based     |
  |   sliders        | +Grim Reaper     | +DJ booth         |  gameplay       |
  |  +8 needs        | +genie lamp      | +costumes         | +console adapt  |
  |  +career ladder  | +crystal ball    | +campfire         | +neighborhood   |
  |  +build/buy mode | +chemistry set   | +celebrity NPCs   |  progression    |
  |  +social system  | +roaches/ghosts  | +mechanical bull   | +unlock system  |
  |  +Simlish        | +voodoo doll     | +bonfire          | +social moves   |
  ─────────────────────────────────────────────────────────────────────────────

  WHAT EACH ERA ADDED TO THE FORMULA:

  SIMS 1: Life exists. Manage it.        (SURVIVAL)
  SIMS 2: Life has depth. Explore it.    (COMPLEXITY)
  SIMS 3: Life has breadth. Travel it.   (WORLD)
  SIMS 4: Life has feeling. Express it.  (EMOTION)
```

---

## 11. THE SUPERNATURAL LAYER -- The Weird Stuff

```
  OCCULT SYSTEMS ACROSS THE FRANCHISE
  =====================================
  (Every era added monsters. Why? Because mundane + strange = compelling.)

  +-------------+------------------+-----------------------------------+
  | CREATURE    | INTRODUCED       | MECHANIC                          |
  +-------------+------------------+-----------------------------------+
  | VAMPIRE     | Sims 2 Nightlife | Bite infects. Sun kills.          |
  |             |                  | Thirst replaces Hunger.           |
  |             |                  | Immortal. 10% population cap.     |
  |             |                  | Coffin sleep. Plasma diet.        |
  +-------------+------------------+-----------------------------------+
  | WEREWOLF    | Sims 2 Pets      | Leader of the Pack bites you.     |
  |             |                  | Nightly transformation.           |
  |             |                  | Personality PERMANENTLY drifts    |
  |             |                  | toward fixed archetype.           |
  |             |                  | Cure does NOT undo the drift.     |
  +-------------+------------------+-----------------------------------+
  | PLANTSIM    | Sims 2 Seasons   | Spray pesticide too much -->      |
  |             |                  | transform into plant person.      |
  |             |                  | 3 needs replace 8 (Sun/Water/Love)|
  |             |                  | Photosynthesis. Asexual reproduce.|
  |             |                  | Auto Gold gardening badge.        |
  +-------------+------------------+-----------------------------------+
  | WITCH       | Sims 2 Apt Life  | NPC witch mentors you.            |
  |             |                  | Alignment: -1000 to +1000.        |
  |             |                  | 30+ spells. Good/Neutral/Evil.    |
  |             |                  | Every spell shifts alignment.     |
  |             |                  | Reagents + cauldron economy.      |
  +-------------+------------------+-----------------------------------+
  | BIGFOOT     | Sims 2 Bon Voy   | Befriend in mountains. Move in.   |
  |             |                  | Fixed personality. Can't change.  |
  +-------------+------------------+-----------------------------------+
  | MUMMY       | Sims 3 World Adv | Guards tombs. Curses intruders.   |
  +-------------+------------------+-----------------------------------+
  | CELEBRITY   | Sims 3 Late Night| Not supernatural but functions    |
  |             |                  | like one: special powers, special |
  |             |                  | vulnerabilities, contagious.      |
  +-------------+------------------+-----------------------------------+

  THE PATTERN:
  +-------------------------------------------------------+
  | Every supernatural creature REPLACES normal systems    |
  | with ALTERNATIVE systems:                              |
  |                                                        |
  | Vampire:  Hunger --> Thirst (alternative fuel)         |
  | PlantSim: 8 needs --> 3 needs (simplified architecture)|
  | Werewolf: Stable personality --> Forced drift          |
  | Witch:    No magic --> Alignment spectrum               |
  | Celebrity: Anonymous --> Reputation economy             |
  |                                                        |
  | THE INSIGHT: The "normal" life template is not the     |
  | only way to exist. The game keeps discovering new      |
  | ways to be alive.                                      |
  +-------------------------------------------------------+
```

---

## 12. THE MONEY MACHINE -- How The Economy Works

```
  THE SIMS ECONOMY
  ==================

  INCOME SOURCES:
  +------------------+------------+------------------+
  | SOURCE           | TYPE       | $/WEEK (Sims 4)  |
  +------------------+------------+------------------+
  | Career salary    | Active     | $2,000-$14,000   |
  | Book royalties   | Passive    | $100-$1,000+     |
  | Painting sales   | Per-item   | $200-$5,000      |
  | Program sales    | Passive    | $100-$500        |
  | Gardening sales  | Harvest    | $50-$2,000       |
  | Fishing sales    | Per-catch  | $10-$500         |
  | Music tips       | Live       | $20-$200/session |
  +------------------+------------+------------------+

  EXPENSES:
  +------------------+------------+
  | Bills (weekly)   | % of lot   |
  | Food             | $10-$50    |
  | Furniture        | one-time   |
  | Repairs          | $50-$200   |
  +------------------+------------+

  THE WEALTH SPIRAL:

       Poor                          Rich
       $1,000                        $100,000+
         |                              |
         v                              v
  +------------+                 +-------------+
  | cheap bed  |                 | best bed    |
  | bad sleep  |                 | great sleep |
  | low energy |                 | high energy |
  | less time  |                 | more time   |
  | slow skills|                 | fast skills |
  | low career |                 | high career |
  | less money |                 | more money  |
  +-----+------+                 +------+------+
        |                               |
        +--- POVERTY TRAP               +--- WEALTH SPIRAL
        (bad stuff makes                 (good stuff makes
         more bad stuff)                  more good stuff)

  THE GUIDE'S ADVICE: Buy the best bed FIRST.
  Sleep quality is the highest-leverage investment.
```

---

## 13. THE TIME BUDGET -- The True Currency

```
  24 HOURS IN A SIM DAY
  =======================
  (Time is the ONLY resource that cannot be bought, earned, or cheated.)

  HOURS:  0  2  4  6  8 10 12 14 16 18 20 22 24
          |  |  |  |  |  |  |  |  |  |  |  |  |
  SLEEP   [########]                    [######]     8 hrs (non-negotiable)
  NEEDS            [###]                             3 hrs (pee/eat/shower)
  WORK                  [##########]                 6 hrs (career)
  COMMUTE               [#]      [#]                 1 hr  (travel)
                                                     ----
                                                     18 hrs LOCKED

  REMAINING: 6 HOURS OF FREE TIME

  YOU MUST CHOOSE:
  +---+---+---+---+---+---+
  | 1 | 2 | 3 | 4 | 5 | 6 |  <-- hours
  +---+---+---+---+---+---+
    |   |   |   |   |   |
    v   v   v   v   v   v
  [SKILL] [SKILL] [SOCIAL] [SOCIAL] [FUN] [FUN]  <-- Option A: balanced
  [SKILL] [SKILL] [SKILL]  [SKILL]  [SK]  [SK]   <-- Option B: grind
  [SOC]   [SOC]   [SOC]    [FUN]    [FUN] [FUN]  <-- Option C: social
  [FUN]   [FUN]   [FUN]    [FUN]    [FUN] [FUN]  <-- Option D: hedonist

  THE OPTIMIZATION:
  +--------------------------------------------------+
  | Don't build a big house   (walking wastes time)   |
  | Don't put rooms upstairs  (stairs waste time)     |
  | Buy a good bed            (less sleep needed)     |
  | Learn to cook             (eating takes less time)|
  | Use multitask objects     (skill + need in one)   |
  |                                                    |
  | Every minute saved on survival = a minute          |
  | gained for meaning.                                |
  +--------------------------------------------------+

  THE PHILOSOPHICAL INSIGHT:
  +--------------------------------------------------+
  | The game makes you feel what real life obscures:   |
  | there are never enough hours.                      |
  |                                                    |
  | You CANNOT max all skills AND have a great career  |
  | AND maintain all friendships AND raise children    |
  | AND keep all needs green.                          |
  |                                                    |
  | Something always gives.                            |
  | Choosing what to sacrifice IS the game.            |
  +--------------------------------------------------+
```

---

## 14. THE LEGACY ARC -- Why You Keep Playing

```
  GENERATIONAL PLAY
  ==================

  Gen 1                Gen 2                Gen 3
  (you built)          (they inherit)       (dynasty)
  +----------+         +----------+         +----------+
  | $20,000  |  --->   | $80,000  |  --->   | $200,000 |
  | 2BR house|         | 4BR house|         | mansion  |
  | 3 skills |         | 5 skills |         | 8 skills |
  | 1 career |         | 2 careers|         | mastery  |
  | starter  |         | growing  |         | dynasty  |
  +----------+         +----------+         +----------+
       |                    |                    |
       v                    v                    v
   struggling           comfortable          wealthy
   surviving            thriving             dominating

  WHAT CARRIES FORWARD:
  - House (physical structure)
  - Money (Simoleons in the bank)
  - Relationships (family tree)
  - Reputation (in later games)
  - Genetics (physical traits)

  WHAT RESETS:
  - Skills (start at 0)
  - Career (start at Level 1)
  - Aspiration (new choice)

  THE HOOK:
  +----------------------------------------------+
  | The first generation is HARD.                 |
  | The second generation is EASIER.              |
  | The third generation is a POWER FANTASY.      |
  |                                                |
  | You're not playing a life.                     |
  | You're building a LINEAGE.                     |
  |                                                |
  | That's why people play for 1000+ hours.        |
  | The investment compounds.                      |
  +----------------------------------------------+
```

---

## 15. WHY IT'S SO POPULAR -- The Complete Picture

```
+=======================================================================+
|                                                                        |
|              WHY THE SIMS IS A $5 BILLION FRANCHISE                    |
|              200 MILLION COPIES. 20+ YEARS. STILL GROWING.             |
|                                                                        |
+=======================================================================+

  1. THE MIRROR
  +----------------------------------------------------------+
  | It reflects YOUR life back at you as a game.              |
  | Chores, jobs, relationships, money, time pressure --      |
  | everything you already deal with, but now you can SEE     |
  | the bars, the numbers, the systems underneath.            |
  |                                                           |
  | "By gamifying the mundane, it reveals how much of         |
  |  real life already operates like a game."                 |
  +----------------------------------------------------------+

  2. THE SANDBOX
  +----------------------------------------------------------+
  | No win condition. No fail state (unless you try).         |
  | No linear story. No "correct" way to play.               |
  |                                                           |
  | Build a family. Burn a house down. Both are valid.        |
  | Create a dynasty. Drown someone in a pool. Both happen.   |
  |                                                           |
  | Freedom without consequence = infinite replayability.     |
  +----------------------------------------------------------+

  3. THE CREATIVITY ENGINE
  +----------------------------------------------------------+
  | Build houses. Design outfits. Create characters.          |
  | Tell stories. Share creations. Download others'.          |
  |                                                           |
  | 41 million uploads. 825 million downloads. Gallery.       |
  | Custom Content. Mods. Let's Plays. Fan fiction.           |
  |                                                           |
  | The game is a PLATFORM. The community is the CONTENT.     |
  +----------------------------------------------------------+

  4. THE OPTIMIZATION PUZZLE
  +----------------------------------------------------------+
  | For the min-maxers: every system can be optimized.        |
  |                                                           |
  | Fastest career path? Interstellar Smuggler.               |
  | Best passive income? Writing books while sleeping.        |
  | Optimal house layout? Bed next to toilet, no stairs.      |
  |                                                           |
  | The game rewards strategic thinking about MUNDANE LIFE.   |
  +----------------------------------------------------------+

  5. THE EMOTIONAL TOYBOX
  +----------------------------------------------------------+
  | Make them fall in love. Make them fight. Make them cry.    |
  | Kill the husband. Remarry. Have an affair.                |
  |                                                           |
  | Players are writing SOAP OPERAS with game mechanics.      |
  | The emotions feel real because the SYSTEMS are real.       |
  +----------------------------------------------------------+

  6. THE POWER FANTASY (inverted)
  +----------------------------------------------------------+
  | Most games: you're a warrior, a hero, a god of war.       |
  | The Sims: you're a god of... laundry. And meals. And      |
  | toilet schedules. And job promotions.                      |
  |                                                           |
  | The power fantasy is CONTROL OVER ORDINARY LIFE.          |
  | That's what most people actually want.                     |
  | Not to slay dragons. To have their shit together.          |
  +----------------------------------------------------------+

  7. THE IDENTITY LAB
  +----------------------------------------------------------+
  | Live a life you can't live.                               |
  | Be someone you aren't.                                    |
  | Try a career you'll never have.                           |
  | Date someone you'd never meet.                            |
  | Build a house you can't afford.                           |
  |                                                           |
  | It's a SAFE SPACE for identity experimentation.           |
  | Representation matters: skin tones, body types,           |
  | same-sex relationships, gender expression.                |
  +----------------------------------------------------------+

  8. THE COMPOUND LOOP
  +----------------------------------------------------------+
  |                                                           |
  |   Create --> Attach --> Invest --> Compound --> Legacy     |
  |      |                                           |        |
  |      +------------ repeat (generations) ---------+        |
  |                                                           |
  |   You build a Sim. You care about them.                   |
  |   You invest time. The investment compounds.              |
  |   They age. They die. Their children inherit.             |
  |   You start caring about the CHILDREN.                    |
  |   The cycle repeats.                                      |
  |                                                           |
  |   THIS is the addiction loop.                             |
  |   Not dopamine hits. ACCUMULATED CARE.                    |
  |   You can't walk away because you BUILT this.             |
  +----------------------------------------------------------+

  THE FINAL INSIGHT:
  +=======================================================+
  |                                                        |
  |  The Sims is not a game about controlling fake people. |
  |                                                        |
  |  It's a game about discovering that YOU are a system.  |
  |  Needs, emotions, skills, relationships, time --       |
  |  you already have all these bars.                      |
  |  You just can't see them.                              |
  |                                                        |
  |  The Sims makes them visible.                          |
  |  And once you see the bars,                            |
  |  you can never unsee them.                             |
  |                                                        |
  +=======================================================+
```

---

*Source: 15 books spanning The Sims franchise (2000-2022)*
*Created: 2026-02-20*
