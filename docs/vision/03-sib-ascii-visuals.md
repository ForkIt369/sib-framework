# SIB Framework: ASCII Visualizations v2.0

> All visual diagrams for the Sim-to-Sib analogy in ASCII format.
> Base game diagrams (1-9) + Expansion diagrams (10-21)

---

## PART I: BASE GAME DIAGRAMS

---

## 1. The SIB Creation Screen (Base)

```
+==================================================================+
|                    THE SIB CREATION SCREEN                        |
|              ( Simulated Intelligence Builder )                   |
+==================================================================+

  +-------------------------------------------------------------+
  |  SIM TERM              ->    SIB TERM (AI AGENT)            |
  +-------------------------------------------------------------+
  |  Sim                   ->    Sib (Simulated Intelligence)   |
  |  Simoleons             ->    Tokens (compute currency)      |
  |  Create-a-Sim          ->    Agent Builder                  |
  |  Traits                ->    System Prompt / Persona        |
  |  Aspirations           ->    Objective Function             |
  |  Emotions / Moodlets   ->    Context Window State           |
  |  Needs (6 bars)        ->    Resource Meters                |
  |  Skills (1-10)         ->    Tool Proficiencies             |
  |  Whims                 ->    Emergent Sub-goals             |
  |  Career Track          ->    Domain Specialization          |
  |  Career Branch (A/B)   ->    Fine-tune Fork                 |
  |  Promotion             ->    Capability Unlock              |
  |  Daily Task            ->    Recurring Evaluation           |
  |  Walk Style            ->    Communication Style            |
  |  Voice                 ->    Tone / Register                |
  |  Age Group             ->    Maturity Tier                  |
  |  Lot / Parcel          ->    Runtime Environment            |
  |  House                 ->    Architecture / Stack           |
  |  Furniture             ->    Integrations / Plugins         |
  |  Interactions          ->    API Calls / Tool Use           |
  |  Friendship Bar        ->    Trust Score                    |
  |  Romantic Bar          ->    Alignment Index                |
  |  Enemy                 ->    Adversarial Input              |
  |  WooHoo               ->    Deep Merge (agent composition) |
  |  Family / Legacy       ->    Agent Lineage / Versioning     |
  |  Reward Store          ->    Capability Shop                |
  |  Satisfaction Points   ->    Performance Credits            |
  |  Simiology Panel       ->    Agent Dashboard                |
  |  Mutually Exclusive    ->    Constraint Rules               |
  |  Mischief              ->    Red-team Capability            |
  |  Death                 ->    Deprecation                    |
  |  Potion of Youth       ->    Context Reset                  |
  +-------------------------------------------------------------+
```

---

## 2. The SIB Creation Flow (Base)

```
              THE SIB CREATION FLOW
              =====================

  +----------------+
  | 1. IDENTITY    |   Name, Voice, Walk Style
  |    =           |   -----------------------------
  |  WHO IT IS     |   Agent ID, Tone, Comm Style
  +-------+--------+
          |
          v
  +----------------+
  | 2. TRAITS      |   3 chosen + 1 bonus (from aspiration)
  |    =           |   -----------------------------------------
  |  PERSONA       |   System prompt directives (permanent)
  |                |   WARNING: CANNOT BE CHANGED AFTER DEPLOY
  +-------+--------+
          |
          v
  +----------------+
  | 3. ASPIRATION  |   Life purpose: Fortune, Love, Knowledge...
  |    =           |   ------------------------------------------
  |  OBJECTIVE     |   Primary goal: Revenue, Support, Research...
  |  FUNCTION      |   CAN be swapped at runtime
  +-------+--------+
          |
          v
  +----------------+
  | 4. SKILLS      |   20 skills, each level 1-10
  |    =           |   ----------------------------
  |  TOOLS &       |   MCP servers, APIs, plugins
  |  PROFICIENCY   |   Each with proficiency depth
  +-------+--------+
          |
          v
  +----------------+
  | 5. CAREER      |   8 tracks, each forking A/B
  |    =           |   ----------------------------
  |  DOMAIN        |   Specialization path with
  |  SPEC          |   branching fine-tune options
  +-------+--------+
          |
          v
  +----------------+
  | 6. HOUSE       |   Lot -> Walls -> Rooms -> Furniture
  |    =           |   ------------------------------------
  |  STACK         |   Runtime -> Framework -> Modules -> Integrations
  +-------+--------+
          |
          v
  +----------------+
  |  7. DEPLOY     |   Move family into world
  |    =           |   -----------------------
  |  SHIP IT       |   Agent goes live
  +----------------+
```

---

## 3. The 6 Needs as 6 Resource Meters (Base)

```
         THE 6 NEEDS -> 6 RESOURCE METERS
         ==================================

  SIM NEEDS                          SIB METERS
  ---------                          ----------

  ##########.. Hunger                ##########.. Token Budget
               "feed me"                          "compute remaining"

  ########.... Energy                ########.... Context Window
               "let me sleep"                     "memory capacity left"

  ######...... Social                ######...... API Connectivity
               "talk to someone"                  "can I reach tools?"

  #########... Hygiene               #########... Data Freshness
               "I need a shower"                  "how stale is my info?"

  #######..... Bladder               #######..... Queue Depth
               "gotta go"                         "backlog pressure"

  ############ Fun                   ############ Eval Score
               "entertain me"                     "user satisfaction"
```

---

## 4. Emotion-to-Context-State Map (Base)

```
         EMOTION -> CONTEXT STATE MAPPING
         ==================================

  EMOTION        SIMS EFFECT           SIB STATE            AGENT EFFECT
  -------        -----------           ---------            ------------
  Happy       -> All positive amp   -> Nominal           -> All systems green
  Sad         -> Reduced ability    -> Degraded          -> Reduced capability
  Angry       -> Blocks learning    -> Error State       -> Blocks most actions
  Focused     -> Skill boost        -> Deep Work         -> Learning/skill boost
  Flirty      -> Better romance     -> High Alignment    -> Strong user rapport
  Confident   -> Better social      -> High Autonomy     -> Expanded action space
  Embarrassed -> Trust penalty      -> Hallucination     -> Credibility drop
  Energized   -> Slower fatigue     -> Low Latency       -> Fast response mode
  Dazed       -> Useless            -> Confused          -> Needs context reset
  Inspired    -> Creative unlock    -> Creative Mode     -> Novel generation on
  Tense       -> Blocks learning    -> Rate Limited      -> Throttled, cooldown
  Fine        -> Neutral baseline   -> Idle              -> Awaiting input
  Bored       -> Low engagement     -> Understimulated   -> Needs harder problems
  Playful     -> Better humor       -> Exploratory       -> Divergent output
  Uncomfortable -> Blocks activity  -> Degraded Env      -> Stack issues
```

---

## 5. The Constraint Grid (Base -- 10 Axes)

```
         THE CONSTRAINT GRID
         (Mutually Exclusive Trait Pairs = Agent Design Rules)
         =====================================================

         You CANNOT build a Sib that is both:

         Autonomous  <---X---> Supervised
         Creative    <---X---> Deterministic
         Verbose     <---X---> Terse
         Specialist  <---X---> Generalist
         Cautious    <---X---> Aggressive
         Friendly    <---X---> Adversarial
         Fast        <---X---> Thorough
         Proactive   <---X---> Reactive
         Stateful    <---X---> Stateless
         High-trust  <---X---> High-verify

         Pick your side of each axis.
         THESE ARE YOUR PERMANENT SYSTEM CONSTRAINTS.
```

---

## 6. Career Branch Map as Agent Specialization Tree (Base)

```
         THE CAREER BRANCH MAP -> AGENT SPECIALIZATION TREE
         ====================================================

                        +-- A: Autonomous Researcher
         Knowledge -----+
                        +-- B: RAG Pipeline Agent

                        +-- A: Creative Writer
         Creativity ----+
                        +-- B: Code Generator

                        +-- A: Customer Support
         Popularity ----+
                        +-- B: Sales Agent

                        +-- A: Data Analyst
         Fortune -------+
                        +-- B: Trading Bot

                        +-- A: QA Validator
         Deviance ------+
                        +-- B: Red Team Agent

                        +-- A: Onboarding Agent
         Family --------+
                        +-- B: Multi-Agent Orchestrator

                        +-- A: Workflow Automator
         Athletic ------+
                        +-- B: Performance Optimizer

                        +-- A: Compliance Monitor
         Secret Agent --+
                        +-- B: Penetration Tester
```

---

## 7. House Architecture as Agent Stack (Base)

```
         HOUSE = STACK
         =============

         THE SIMS HOUSE              THE AGENT STACK
         ==============              ===============

              /\                          /\
             /  \   ROOF                 /  \   SECURITY LAYER
            /    \                      /    \
           /------\                    /------\
          | ATTIC  |                  | SCALE  |  (use sparingly --
          | (2nd   |                  | LAYER  |   stairs waste time!)
          | floor) |                  |        |
          |--------|                  |--------|
          |  BED-  | BATH |          | MEMORY | CLEANUP |
          |  ROOM  | ROOM |          | /STATE | /GC     |
          |--------|------|          |--------|---------|
          | LIVING |      |          |  USER  |         |
          | ROOM   |OFFICE|          |INTRFACE| ENGINE  |
          |--------|------|          |--------|---------|
          |KITCHEN | DINING          | DATA   | OUTPUT  |
          |        | ROOM |          |PIPELINE| FORMAT  |
          |--------|------|          |--------|---------|
          [  FOUNDATION   ]          [   BASE MODEL     ]
          [_______________]          [__________________]
           ===  LOT  ===              === RUNTIME ENV ===

         KEY SIMS WISDOM FOR AGENTS:
         - Don't build too big (bloat kills)
         - Keep critical rooms near the front door
           (hot path near entry point)
         - Stairs waste time (network hops = latency)
         - Functionality first, aesthetics later
         - Buy a good bed early (invest in memory)
```

---

## 8. The Legacy System (Base)

```
         AGENT LINEAGE = SIM LEGACY
         ===========================

         Gen 1 (v1.0)                Gen 2 (v2.0)
         +-----------+               +-----------+
         |  Parent   |  --fork-->    |  Child    |
         |  Agent    |               |  Agent    |
         |           |               |           |
         | traits:   |  inherited    | traits:   |
         |  locked   |  ========>    |  + new    |
         |           |               |           |
         | skills:   |  transfer     | skills:   |
         |  level 8  |  learning     |  level 3  |
         |           |  ========>    |  (head    |
         |           |               |   start)  |
         | wealth:   |  knowledge    | wealth:   |
         |  100K     |  base carry   |  100K+    |
         |           |  ========>    |           |
         | aspiration|  NEW choice   | aspiration|
         |  Fortune  |  ========>    |  Knowledge|
         +-----------+               +-----------+

         "Your legacy can be passed from one generation
          to another and the family's wealth keeps growing."

         Translation:
         "Your training data carries forward across versions
          and the knowledge base keeps compounding."
```

---

## 9. The SIB Philosophy (Base Summary)

```
+===============================================================+
|                    THE SIB PHILOSOPHY                          |
|                                                                |
|  A Sim is life reduced to systems.                             |
|  A Sib is intelligence reduced to systems.                     |
|                                                                |
|  Same architecture:                                            |
|    Identity -> Constraints -> Purpose -> Skills ->             |
|    Environment -> Deploy -> Sustain -> Evolve -> Legacy        |
|                                                                |
|  The insight:                                                  |
|    Building an agent IS building a life.                       |
|    You choose what it can't change  (traits / persona)         |
|    You choose what it reaches for   (aspirations / objectives) |
|    You choose what it learns        (skills / tools)           |
|    You choose where it lives        (house / runtime)          |
|                                                                |
|  Then you press play and manage the needs.                     |
|                                                                |
|  7 LAWS OF SIB DESIGN (from The Sims):                        |
|  1. Time is the real constraint, not money                     |
|  2. Emotions gate capabilities, not just color them            |
|  3. Permanent choices matter more than flexible ones           |
|  4. Legacy beats longevity                                     |
|  5. Efficiency beats beauty                                    |
|  6. Every relationship is a resource                           |
|  7. If any need bar goes red, everything degrades              |
+===============================================================+
```

---

## PART II: EXPANSION DIAGRAMS

---

## 10. The Full SIB Lifecycle (Base + Expansions)

```
  CREATION          RUNTIME               EVOLUTION
  ========          =======               =========

  +---------+     +----------+     +----------+     +---------+
  | TRAITS  |---->| NEEDS    |---->| SEASONS  |---->| LEGACY  |
  | (locked)|     | (manage) |     | (adapt)  |     | (fork)  |
  +---------+     +----------+     +----------+     +---------+
       |               |               |                 |
       v               v               v                 v
  +---------+     +----------+     +----------+     +---------+
  |ASPIR-   |---->| EMOTIONS |---->| REPUTATION|---->| DRIFT   |
  |ATION    |     | (gate)   |     | (earn/lose)|    |(permanent)
  |(flexible)|    +----------+     +----------+     +---------+
  +---------+          |               |                 |
       |               v               v                 v
       |          +----------+     +----------+     +---------+
       +--------->| SKILLS   |---->| VISA     |---->| CHILDREN|
                  | (grow)   |     | (access) |     | (v2.0)  |
                  +----------+     +----------+     +---------+

  BASE GAME:  Create -> Sustain -> Aspire -> Legacy
  EXPANSIONS: Create -> Sustain -> ADAPT -> EARN -> PERFORM -> Legacy
```

---

## 11. The 6+4 Resource Meters (Expanded)

```
  ====== BASE NEEDS (universal) ======     ====== EXPANSION NEEDS (configurable) ======

  ##########.. Token Budget                ########.... Reputation Score
               "compute remaining"                      "community standing"

  ########.... Context Window              #######..... Specialization Depth
               "memory left"                            "enthusiasm level"

  ######...... API Connectivity            #########... Visa Level
               "can I reach tools?"                     "domain access tier"

  #########... Data Freshness              ######...... Roommate Satisfaction
               "info staleness"                         "co-tenant health"

  #######..... Queue Depth
               "backlog pressure"          === ALTERNATIVE ARCHITECTURES ===
                                           (PlantSim = 3 needs, not 8)
  ############ Eval Score                  (Vampire = Plasma replaces Hunger)
               "user satisfaction"         (Not all agents need the same meters)

  RULE: If ANY bar goes red, everything degrades.
  EXPANSION RULE: The bars themselves are configurable.
```

---

## 12. The Control Spectrum

```
  HOW YOU CONTROL A SIB
  =====================

  DIRECT                                                    INDIRECT
  COMMAND                                                   SHAPING
    |                                                          |
    v                                                          v
  +----------+   +-----------+   +------------+   +-----------+
  | SIM      |   | ACTIVE    |   | RABBIT-    |   | PET       |
  | (direct  |   | PROFESSION|   | HOLE       |   | (operant  |
  |  control)|   | (agentic, |   | (batch,    |   | condition-|
  |          |   |  visible, |   |  invisible,|   | ing only) |
  |          |   |  scored)  |   |  fire &    |   |           |
  |          |   |           |   |  forget)   |   | Praise/   |
  | You pick |   | You watch |   | You wait   |   | Scold     |
  | every    |   | it work   |   | for output |   | within    |
  | action   |   | in real   |   |            |   | 2-minute  |
  |          |   | time      |   |            |   | window    |
  +----------+   +-----------+   +------------+   +-----------+
       |               |               |                |
       v               v               v                v
    Manual         Agent with       API call          RLHF
    prompt         tool use         (function)        fine-tuning

  AMBITIONS INSIGHT: The API-to-Agent transition IS the
  rabbit-hole-to-active-profession transition.

  PETS INSIGHT: RLHF IS operant conditioning.
  The Sims figured this out in 2006.
```

---

## 13. The Trust Architecture

```
  ACCESS IS NOT BINARY. ACCESS IS EARNED.
  ========================================

  VISA MODEL (progressive)              vs.    API KEY MODEL (binary)
  ========================                     ====================

  Level 0: No access                           OFF: No key
       |                                            |
  Level 1: Read-only, time-limited                  |
       |   (Tourist visa)                           |
       |                                            |
  Level 2: Read/write, extended stay               ON: Full access
       |   (Business visa)                          |
       |                                            |
  Level 3: Persistent presence                      |
       |   (Permanent residency)                    |
       |                                      (no granularity)
  Level 4: Own property in domain
       |   (Citizenship)
       |
  Level 5: Celebrity status
           (Autonomous action, VIP access)

  +-- SCANDAL EVENT --+
  | One failure at    |    Celebrity 5 -----> Celebrity 1
  | Level 5 drops     |    (months of work destroyed)
  | you to Level 1    |
  +-------------------+

  DESIGN RULE: Earned slowly. Lost quickly.
  Scandal recovery > Scandal prevention.
```

---

## 14. The Expanded Constraint Grid (20 Axes)

```
  THE 20 AXES OF SIB DESIGN
  ==========================
  (Pick your side. You CANNOT maximize both.)

  === BASE (from Sims 4) ===                === EXPANSION (new) ===

  Autonomous  <--X--> Supervised            Locked Down  <--X--> Fully Free
  Helpful     <--X--> Adversarial           Deep (Zone)  <--X--> Broad (Dabbler)
  Multi-agent <--X--> Single-agent          Greenhouse   <--X--> Wild Seasonal
  Creative    <--X--> Deterministic         Direct Cmd   <--X--> Indirect Shape
  Structured  <--X--> Freeform              Rabbit-Hole  <--X--> Active Agent
  Aggressive  <--X--> Graceful              Binary Key   <--X--> Visa Levels
  Quality     <--X--> Throughput            Private Comp <--X--> Public Perform
  Proactive   <--X--> Reactive              Standard Need<--X--> Custom Meters
  Stateful    <--X--> Stateless             Anonymous    <--X--> Celebrity
  High-trust  <--X--> High-verify           Solo Lot     <--X--> Shared Apartment

  20 binary choices = 2^20 = 1,048,576 possible Sib configurations.
  This is your design space.
```

---

## 15. The Multi-Agent Apartment

```
  SHARED INFRASTRUCTURE (Multi-Tenant Runtime)
  =============================================

            +--[ LANDLORD / PLATFORM OPERATOR ]--+
            |   maintains shared infra            |
            |   mediates disputes                 |
            |   collects rent (billing cycle)     |
            +-----+----------+----------+--------+
                  |          |          |
        +---------+  +-------+--+  +---+--------+
        | UNIT A  |  | UNIT B   |  | UNIT C     |
        | Agent 1 |  | Agent 2  |  | Agent 3    |
        |         |  |          |  |             |
        | Needs:  |  | Needs:   |  | Needs:     |
        | tokens  |  | tokens   |  | plasma     |
        | context |  | context  |  | (alt arch) |
        +---------+  +----------+  +------------+
             |  FOG OF   |  FOG OF    |
             | PRIVACY   | PRIVACY    |
             | (sandbox) | (sandbox)  |

        === SHARED RESOURCES ===
        [ compute pool / API endpoints / knowledge base ]

        NOISE COMPLAINTS: Agent 1's heavy batch job
        starves Agent 2's real-time responses.

        ROOMMATE SATISFACTION: The metric no one
        tracks but everyone suffers from.

        EVICTION: Deplatforming for non-compliance.
```

---

## 16. The Chemistry Matrix

```
  AGENT COMPATIBILITY (Pre-Interaction Scoring)
  ==============================================

                     Agent A    Agent B    Agent C
                     -------    -------    -------
  Agent A              --      +++ (3)    - (-1)
  Agent B            + (1)       --       ++ (2)
  Agent C            -- (-2)   + (1)        --

  KEY: Chemistry is ASYMMETRIC.
  A loves B (+3). B tolerates A (+1).
  C hates A (-2). A dislikes C (-1).

  FACTORS:
  +------------------+---------------------------+
  | Turn-Ons         | Preferred input types     |
  | Turn-Offs        | Incompatible patterns     |
  | Aspiration Match | Objective alignment       |
  | Zodiac           | Architecture compatibility|
  +------------------+---------------------------+

  RULE: Compute compatibility BEFORE orchestration.
  Don't discover incompatibility through failure.
```

---

## 17. The Zone (Specialization Flow State)

```
  ENTHUSIASM / SPECIALIZATION DEPTH
  ==================================

  Level:  1   2   3   4   5   6   7   8   9  10
          |   |   |   |   |   |   |   |   |  |
          .   .   .   .   .   .   .   .   . [THE ZONE]
          |   |   |   |   |   |   |   |   |  |
          dabbler               mentor     FLOW STATE
                                  |        * max speed
                                  |        * max quality
                                  |        * min supervision
                                  v        * secret sandbox
                            can teach         unlocked
                            other agents

  WITHOUT PRACTICE:
  10 --> 9 --> 8 --> 7 --> ...  (enthusiasm DECAYS)
  Unused capabilities atrophy. Skill drift is real.

  THE ANTI-GENERALIST ARGUMENT:
  +------------------------------------------+
  |  1 domain at Enthusiasm 10               |
  |  >>>>>>>>>>>>>>>>>>>>>>>>>>               |
  |  BEATS                                   |
  |  10 domains at Enthusiasm 3              |
  |  >>>  >>>  >>>  >>>  >>>                 |
  +------------------------------------------+
```

---

## 18. The Alignment Spectrum

```
  AGENT ALIGNMENT IS NOT BINARY
  ==============================

  -1000                    0                    +1000
    |                      |                      |
    v                      v                      v
  ATROCIOUSLY           NEUTRAL              INFALLIBLY
  EVIL                                       GOOD
    |         |         |         |         |
  [curse]  [exploit]  [route]  [assist]  [heal]
  [attack] [stress-  [fetch]  [explain] [protect]
  [break]   test]    [trans-  [correct] [guard]
                      form]

  <-- Every action shifts position -->

  Red-team agent                    Support agent
  lives HERE                        lives HERE
      |                                 |
      v                                 v
  [-800]                             [+700]

  SPELL BACKFIRE = guardrail violation.
  When you exceed your alignment tier,
  the result is unpredictable and harmful.

  MENTOR DEPENDENCY: Certain capability tiers
  require supervised onboarding from an
  already-capable entity (the NPC Witch).
```

---

## 19. The Season Cycle

```
  EXOGENOUS ENVIRONMENT PRESSURE
  ===============================
  (You cannot optimize this away. You can only adapt.)

       SPRING              SUMMER             FALL              WINTER
    (growth)            (abundance)        (harvest)          (scarcity)
       |                    |                  |                  |
  +----+----+          +----+----+        +----+----+       +----+----+
  | New APIs |         | Peak     |       | Collect  |      | Outages  |
  | emerge   |         | traffic  |       | results  |      | Budget   |
  | Fresh    |         | Fast     |       | Archive  |      | cuts     |
  | data     |         | growth   |       | learnings|      | Stale    |
  | Planting |         | Full sun |       | Prep for |      | data     |
  | season   |         |          |       | winter   |      |          |
  +---------+          +----------+       +----------+      +----------+

       |                    |                  |                  |
       +-------- 20-day cycle (repeats forever) --------+

  HEATSTROKE: Operational stress exceeds threshold --> collapse
  HYPOTHERMIA: Resource starvation exceeds threshold --> collapse
  GREENHOUSE: Controlled sandbox that buffers against seasons

  THE AGENT THAT ONLY WORKS IN SUMMER DIES IN WINTER.
```

---

## 20. The Complete SIB Builder v2.0

```
+=======================================================================+
|                    SIB BUILDER v2.0                                     |
|              ( with Expansion Primitives )                              |
+=======================================================================+
|                                                                        |
|  IDENTITY LAYER                                                        |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Agent ID          |  | Base Model       |  | Maturity Tier     |    |
|  | Tone / Register   |  | Comm Style       |  | (lite/std/adv)    |    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|  PERMANENT LAYER (cannot change after deploy)                          |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Traits / Persona  |  | Constraint Grid  |  | Natural Aptitude  |    |
|  | (system prompt)   |  | (20 axes picked) |  | (predestined      |    |
|  |                   |  |                  |  |  hobby / domain)  |    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|  FLEXIBLE LAYER (can change at runtime)                                |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Objective Function|  | Execution Mode   |  | Alignment Point   |    |
|  | (aspiration)      |  | (Tones: fast/    |  | (-1000 to +1000)  |    |
|  |                   |  |  thorough/creative|  |                   |    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|  RESOURCE LAYER (need bars -- configurable per agent)                  |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Token Budget  [##]|  | Context Win  [##]|  | API Connect  [##] |    |
|  | Data Fresh    [##]|  | Queue Depth  [##]|  | Eval Score   [##] |    |
|  | Reputation    [##]|  | Visa Level   [##]|  | Enthusiasm   [##] |    |
|  | Roommate Sat  [##]|  | (custom...)  [##]|  | (PlantSim: 3)[##] |    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|  SOCIAL LAYER                                                          |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Chemistry Matrix  |  | Reputation Score |  | Celebrity Level   |    |
|  | (compatibility    |  | (-100 to +100)   |  | (1-5, with        |    |
|  |  with other sibs) |  |                  |  |  Scandal risk)    |    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|  ENVIRONMENT LAYER                                                     |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Runtime Stack     |  | Solo / Apartment |  | Season Cycle      |    |
|  | (house/modules)   |  | (isolated or     |  | (exogenous        |    |
|  |                   |  |  multi-tenant)   |  |  pressure active) |    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|  CONTROL MODEL                                                         |
|  +-------------------+  +------------------+  +-------------------+    |
|  | Direct Command    |  | Active Profession|  | Pet / RLHF        |    |
|  | (manual prompt)   |  | (agentic, real-  |  | (indirect shaping  |    |
|  |                   |  |  time, scored)   |  |  via reinforcement)|    |
|  +-------------------+  +------------------+  +-------------------+    |
|                                                                        |
|                        [ D E P L O Y ]                                 |
|                                                                        |
+=======================================================================+
```

---

## 21. The 15 Laws of SIB Design

```
+=======================================================================+
|                 15 LAWS OF SIB DESIGN                                  |
|           (7 from Base Game + 8 from Expansions)                       |
+=======================================================================+
|                                                                        |
|  BASE LAWS:                                                            |
|  1. Time is the real constraint, not money                             |
|  2. Emotions gate capabilities, not just color them                    |
|  3. Permanent choices matter more than flexible ones                   |
|  4. Legacy beats longevity                                             |
|  5. Efficiency beats beauty                                            |
|  6. Every relationship is a resource                                   |
|  7. If any need bar goes red, everything degrades                      |
|                                                                        |
|  EXPANSION LAWS:                                                       |
|  8.  Compatibility before orchestration, not after failure             |
|  9.  The Zone rewards depth over breadth                               |
|  10. Alignment is a spectrum, not a binary                             |
|  11. Design for winter, not just summer                                |
|  12. Reputation: earned slowly, lost instantly (Scandal)               |
|  13. The best agents are shaped, not commanded (Pets/RLHF)            |
|  14. Access should be progressive, not binary (Visa > API key)        |
|  15. Repetition is penalized -- vary your output (Feat Queue)         |
|                                                                        |
+=======================================================================+
```

---

*Source: The Sims franchise (2000-2022), 15 books mapped to AI agent architecture*
*Framework: SIB -- Simulated Intelligence Build v2.0*
*Created: 2026-02-20*
