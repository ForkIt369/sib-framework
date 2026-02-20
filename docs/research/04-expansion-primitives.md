# SIB Expansion Primitives

> New concepts from The Sims expansion packs (Sims 1, 2, 3) that extend the base SIB framework into deeper agent design territory. Everything here is additive -- the base Sims 4 mappings in `02-sib-analogy-map.md` remain unchanged.

---

## I. NEW PRIMITIVES

### 1. Chemistry / Attraction System
**Sim Mechanic:** Nightlife introduced a multi-factor compatibility score between Sims -- Turn-Ons, Turn-Offs, Aspiration match, Zodiac compatibility -- producing a -3 to +3 "bolt" rating. Chemistry is asymmetric: Sim A's attraction to Sim B can differ from B's attraction to A.

**SIB Mapping: Agent Compatibility Matrix**
Agents working in multi-agent systems need a compatibility function that determines how well two agents collaborate. This is not the same as the base framework's Trust Score (relationship bar). Chemistry is *pre-interaction* -- a structural compatibility assessment computed from configuration overlap before any work begins.

| Chemistry Factor | Agent Equivalent |
|---|---|
| Turn-Ons (2 per Sim) | Preferred Input Types (e.g., prefers structured data, prefers natural language) |
| Turn-Offs (1 per Sim) | Incompatible Patterns (e.g., rejects unstructured blobs, cannot process images) |
| Aspiration Match | Objective Alignment (are both agents optimizing for the same meta-goal?) |
| Zodiac Compatibility | Architecture Compatibility (do their base models, context window sizes, and tool sets mesh?) |
| Bolt Rating (-3 to +3) | Collaboration Score (computed before pairing, predicts coordination efficiency) |
| Asymmetric Chemistry | Asymmetric Utility (Agent A benefits more from Agent B than B benefits from A) |

**Design Principle:** Not all agents work well together. Compatibility should be computed before orchestration, not discovered through failure.

---

### 2. Hobby Enthusiasm / The Zone
**Sim Mechanic:** FreeTime introduced 10 hobbies with a 1-10 enthusiasm meter. Enthusiasm grows with repeated engagement, decays with inactivity. At Enthusiasm 10, a Sim enters "The Zone" -- a visible flow state that accelerates output quality and speed. Each Sim has a Predestined Hobby determined by personality traits.

**SIB Mapping: Specialization Depth / Flow State**

| Enthusiasm Element | Agent Equivalent |
|---|---|
| Enthusiasm Meter (1-10) | Specialization Depth -- how much repeated practice an agent has in a narrow domain |
| Enthusiasm Decay | Skill Atrophy -- unused capabilities degrade (model drift, stale fine-tuning) |
| Predestined Hobby | Natural Aptitude -- base model architecture predisposes certain agents toward certain tasks |
| The Zone (Enthusiasm 10) | Flow State -- when an agent operates in its deepest specialization, it produces faster, higher-quality output with less supervision |
| Instruct in Hobby (6+) | Mentoring -- a highly specialized agent can accelerate another agent's learning in the same domain |
| Secret Hobby Lot | Specialist Sandbox -- hidden environments/datasets that only unlock at peak specialization |

**Design Principle:** Breadth is not depth. An agent that does one thing at Enthusiasm 10 outperforms an agent that does ten things at Enthusiasm 3. The Zone rewards commitment. This is the anti-generalist argument in agent design.

---

### 3. Witchcraft Alignment Spectrum
**Sim Mechanic:** Apartment Life introduced a -1000 to +1000 alignment spectrum with 7 levels from Atrociously Evil to Infallibly Good. Every spell cast shifts alignment. Good, Neutral, and Evil paths each have different spellbooks, different capabilities, different summoned entities.

**SIB Mapping: Agent Alignment Spectrum**

| Witchcraft Element | Agent Equivalent |
|---|---|
| Alignment (-1000 to +1000) | Safety/Autonomy Spectrum -- how constrained vs. free-acting an agent is |
| 7 alignment levels | Guardrail Tiers (e.g., Locked Down / Cautious / Moderate / Balanced / Flexible / Autonomous / Unconstrained) |
| Good Spells (heal, beautify) | Assistive Actions (help, explain, correct) |
| Evil Spells (curse, attack) | Adversarial Actions (red-team, exploit, stress-test) |
| Neutral Spells (utility) | General-Purpose Actions (fetch, transform, route) |
| Every spell shifts alignment | Every action shifts the agent's behavioral history, which should inform future trust calibration |
| Spell backfire on failure | Guardrail violation -- when an agent exceeds its alignment, the result is unpredictable and often harmful |
| NPC Witch required to transform | Mentor Dependency -- certain capability tiers require supervised onboarding from an already-capable entity |

**Design Principle:** Alignment is not binary (safe/unsafe). It is a spectrum, and every action shifts where an agent sits on it. A red-team agent and a customer-support agent need different alignment profiles. The spectrum, not the binary, is the design primitive.

---

### 4. Season Cycle / Environmental Pressure
**Sim Mechanic:** Seasons introduced a 20-day cycle (Spring/Summer/Fall/Winter) with weather, temperature, crop growth, and seasonal interaction availability. Internal Temperature (-100 to +100) creates heatstroke and hypothermia risk. The environment affects everything but is controlled by nothing.

**SIB Mapping: Exogenous Environment Cycling**

| Season Element | Agent Equivalent |
|---|---|
| Season Cycle (20 days) | Market/Demand Cycles -- periodic shifts in what users need, what data is fresh, what APIs are available |
| Weather (rain, snow, heat) | External Conditions -- API rate limits, model provider outages, cost fluctuations, regulatory changes |
| Internal Temperature | Operational Stress -- a hidden stat tracking cumulative environmental pressure on the agent |
| Heatstroke / Hypothermia | Stress Failure -- when operational stress exceeds thresholds, the agent collapses |
| Greenhouse (indoor growing) | Controlled Environment -- staging/sandbox environments that buffer against external volatility |
| Seasonal Crop Bonuses | Timing Advantage -- some tasks yield better results at certain points in the cycle (batch processing overnight, launching features on slow days) |
| Give Gift Winter Bonus (+20) | Contextual Amplifiers -- certain actions are worth more in certain environmental states |

**Design Principle:** The most powerful variable is the one you cannot control. Agents must be designed for seasonal variance -- not just steady-state optimization but adaptation to cyclical environmental pressure. The agent that only works in summer dies in winter.

---

### 5. Celebrity / Fame / Reputation System
**Sim Mechanic:** Late Night introduced a 5-level Celebrity system with escalating perks and vulnerabilities. Apartment Life added a -100 to +100 Reputation with 9 levels. Both are persistent, neighborhood-wide, and affect every social interaction.

**SIB Mapping: Agent Reputation Layer**

| Fame/Reputation Element | Agent Equivalent |
|---|---|
| Celebrity Level (1-5) | Trust Tier -- escalating levels of access granted by users/systems based on demonstrated performance |
| Star Treatment Perks | Privilege Escalation -- higher trust tiers unlock capabilities (write access, production deployment, autonomous action) |
| Paparazzi | Audit Trail -- at higher trust levels, more logging and monitoring are applied |
| Scandal | Trust Collapse Event -- a single failure at high trust level causes disproportionate reputation damage |
| Bouncer / VIP Gating | Access Control -- certain resources/APIs/environments require minimum trust level |
| Reputation Score (-100 to +100) | Community Standing -- an aggregate score across all users/systems that modifies interaction acceptance globally |
| "Do You Know Who I Am?" | Credential Assertion -- invoking reputation to bypass normal access controls |
| 10% Vampire Cap | Population Control -- limiting how many agents can hold a given privilege level to prevent system degradation |

**Design Principle:** Reputation is earned slowly and lost quickly. The Scandal mechanic is the critical insight: high-trust agents have more to lose, and a single failure event can undo months of earned reputation. Design for graceful scandal recovery, not just scandal prevention.

---

### 6. Pet AI / Non-Player Autonomous Agents
**Sim Mechanic:** Pets introduced creatures you cannot directly control that cohabit with Sims and operate under their own behavioral logic. Pets learn through operant conditioning (Praise/Scold within a 2-minute reinforcement window) across 8 behavioral axes.

**SIB Mapping: Sub-Agents / Indirectly Controlled Entities**

| Pet Element | Agent Equivalent |
|---|---|
| Pet (uncontrollable agent) | Sub-Agent -- an entity in the system you configure but do not directly command |
| 8 Reinforceable Behaviors | Behavioral Axes -- configurable dimensions of sub-agent behavior shaped through feedback |
| Praise / Scold | Positive/Negative Reinforcement Signal -- RLHF-style feedback that shifts behavioral meters |
| 2-Minute Reinforcement Window | Feedback Latency Constraint -- reinforcement must be temporally proximate to the behavior it targets |
| Training Meter (-100 to +100) | Behavioral Drift Score -- how far a sub-agent has been shaped from its baseline |
| Pack / Master / Mine bonds | Attachment Hierarchy -- sub-agents form different types of loyalty bonds with different principals |
| Pet Career (Security/Service/Showbiz) | Sub-Agent Specialization Track -- even indirectly controlled entities can develop domain expertise |
| Teachable Commands | Callable Functions -- discrete operations the sub-agent learns to execute on demand |
| Ownership Points | Authority Accumulation -- which principal has the most influence over the sub-agent |

**Design Principle:** The most interesting agents in a system are the ones you cannot directly control. Pets teach that indirect control through systematic reinforcement -- not direct command -- is a valid and sometimes superior architecture. RLHF is operant conditioning for language models. The Sims figured this out in 2006.

---

### 7. Apartment Shared-Space Dynamics
**Sim Mechanic:** Apartment Life introduced multi-household lots with Landlords, rent, Roommate Satisfaction (-100 to +100), noise/smell complaints, and Fog of Privacy between units.

**SIB Mapping: Multi-Tenant Runtime Environment**

| Apartment Element | Agent Equivalent |
|---|---|
| Apartment Building | Shared Infrastructure (multi-tenant cloud, shared API endpoints, common compute pools) |
| Landlord | Platform Operator -- the entity that maintains shared infrastructure and mediates disputes |
| Rent (weekly, with grace period) | Resource Quota / Billing Cycle -- periodic compute costs that must be paid or the agent gets evicted |
| Roommate Satisfaction | Co-Tenant Health -- how well multiple agents sharing resources affect each other |
| Noise Complaints | Resource Contention -- one agent's heavy usage degrading another's performance |
| Fog of Privacy | Isolation / Sandboxing -- preventing agents from seeing each other's internal state |
| Rent Discount for Befriending Landlord | Relationship-Based Pricing -- better terms for agents that maintain good standing with the platform |
| Eviction | Deplatforming -- removal from shared infrastructure for non-compliance |

**Design Principle:** Most agents do not run in isolation. They share infrastructure, and shared infrastructure creates friction. Roommate Satisfaction is the metric no one tracks but everyone suffers from: how does your agent's resource usage affect co-tenants?

---

### 8. Visa / Travel System
**Sim Mechanic:** Bon Voyage (Sims 2) and World Adventures (Sims 3) introduced travel destinations gated by Visa Levels. Higher visa levels allow longer stays, deeper access, and eventually permanent real estate. Visas are earned through activity at the destination.

**SIB Mapping: Cross-Domain Access Credentials**

| Travel Element | Agent Equivalent |
|---|---|
| Destination (China/France/Egypt) | External Domain (different APIs, data sources, or specialized environments) |
| Visa Level (1-3) | Access Tier -- progressively deeper permissions earned through demonstrated competence in the domain |
| Visa Points | Domain Reputation -- accumulated evidence of successful operation in a foreign domain |
| Certificate of Partnership | Extended Access Token -- temporary override allowing deeper access than the visa level normally permits |
| Vacation Home (Visa Lv3) | Persistent Domain Footprint -- at maximum access, the agent maintains a permanent presence in the external domain |
| Cross-Destination Adventures | Cross-Domain Workflows -- tasks that span multiple external domains, requiring credentials in each |
| Vacation Score (Carefree/Refreshed/Productive) | Domain Mission Quality -- scored assessment of how effectively the agent operated in the foreign domain |

**Design Principle:** Access to foreign domains should be progressive, not binary. An agent earns its way into deeper access through demonstrated competence. The visa model is superior to the API-key model: instead of "you have access or you don't," it is "you have Level 1 access, and you earn Level 3."

---

### 9. Active Professions
**Sim Mechanic:** Ambitions replaced passive "rabbit-hole" careers with Active Professions where the player directly controls the Sim during work. Ghost Hunter, Firefighter, Investigator, Architectural Designer, and Stylist each have real-time task execution, client evaluation, and visible scoring.

**SIB Mapping: Agentic Work vs. Passive Processing**

| Active Profession Element | Agent Equivalent |
|---|---|
| Rabbit-Hole Career (passive) | Batch Processing -- send input, wait for output, no visibility into execution |
| Active Profession (real-time) | Agentic Execution -- the agent operates in the environment in real-time, making decisions as it works |
| Client Evaluation Scoring | User Feedback Loop -- work product is evaluated against explicit criteria, not just "did it complete" |
| Portfolio System | Work History -- a tracked record of past outputs that demonstrates capability progression |
| Tones (Work Hard / Take It Easy) | Execution Mode -- configurable behavioral posture during task execution (thorough vs. fast, precise vs. creative) |
| Skill-Based Self-Employment | Freelance Agent -- monetizing capability directly rather than operating within an organizational career track |

**Design Principle:** The shift from rabbit-hole to active profession is the shift from API to agent. An API disappears into a building and returns a result. An agent operates visibly in the world, makes real-time decisions, and is scored on how it works, not just what it produces.

---

### 10. Performance / Stage System
**Sim Mechanic:** Showtime introduced stage careers (Singer, Magician, Acrobat) where performers queue Feats from a library, are scored on variety and execution, and progress through venue tiers from Parks to Big Shows. Feat repetition is penalized; risk-taking is rewarded.

**SIB Mapping: Agent Output as Performance**

| Performance Element | Agent Equivalent |
|---|---|
| Feat Library | Capability Repertoire -- the set of operations an agent can perform |
| Feat Queue (set list) | Execution Plan -- the ordered sequence of operations for a given task |
| Variety Scoring | Diversity Bonus -- penalizing repetitive/templated output, rewarding novel approaches |
| Venue Tier (Park to Big Show) | Deployment Context Tier -- the stakes/visibility of the environment the agent is operating in |
| SimFest (competition) | Benchmark / Eval -- competitive evaluation against other agents on the same task |
| Stage FX Theme Matching | Context Coherence -- bonus for matching output style to the deployment context |
| Hidden Performance Skill | Implicit Quality -- a latent capability metric that improves with practice but is not directly observable |

**Design Principle:** Repetition is penalized. An agent that produces the same output pattern every time is the equivalent of a performer repeating the same feat -- the audience (user) loses interest. Variety in execution is a scorable quality.

---

## II. NEW LEXICON

Terms from the expansions that map onto agent concepts with precision.

| Expansion Term | Source | SIB Mapping | Definition |
|---|---|---|---|
| **Chemistry Bolts** | Nightlife | Compatibility Score | Pre-interaction structural compatibility rating between two agents |
| **The Zone** | FreeTime | Flow State | Peak specialization state where output quality and speed are maximized |
| **Predestined Hobby** | FreeTime | Natural Aptitude | The task domain a model architecture is inherently best suited for |
| **Enthusiasm Decay** | FreeTime | Skill Atrophy | Unused capabilities degrade over time |
| **Furious State** | Nightlife | Emotional Debt | Temporary extreme negative state with time-decay; caused by trust violation |
| **Rivalry** | Nightlife | Agent Competition | Two agents competing for the same resource/attention, autonomously interfering with each other |
| **Fog of Privacy** | Apartment Life | Sandboxing | Isolation layer preventing agents from observing each other's internal state |
| **Social Class** | Apartment Life | Resource Tier | Economic classification that determines which capabilities and environments are accessible |
| **Social Group** | Apartment Life | Tribal Affiliation | Agents that share a group identity get networking bonuses in their career domain |
| **Reputation** | Apartment Life | Community Standing | Persistent, cross-context score that modifies every interaction acceptance rate |
| **Scandal** | Late Night | Trust Collapse Event | Single failure at high reputation that causes disproportionate score loss |
| **Bouncer** | Late Night | Access Gate | An entity that checks credentials before allowing access to a resource |
| **Visa Level** | World Adventures | Progressive Domain Access | Earned-through-use access tier for foreign domains |
| **Adventure Board** | World Adventures | Task Queue / Opportunity Board | A structured source of available tasks that chain into sequences |
| **Tomb** | World Adventures | Puzzle Pipeline | A multi-step, gated problem-solving environment with traps and rewards |
| **Keystone Panel** | World Adventures | Authentication Gate | A lock requiring a specific matching credential to proceed |
| **Floor Switch** | World Adventures | Trigger Event | A condition that, when met, unlocks the next step in a pipeline |
| **Dive Well** | World Adventures | Cross-Layer Transport | A mechanism for moving between levels/layers of a system |
| **Memento Rack of Glory** | Bon Voyage | Capability Trophy Case | Accumulated evidence of cross-domain experience that confers passive bonuses |
| **Vacation Score** | Bon Voyage | Mission Quality Rating | Scored assessment of how effectively an agent operated in a foreign environment |
| **Pack / Master / Mine** | Pets | Attachment Hierarchy | Different types of loyalty bonds between sub-agents and their principals |
| **Training Meter** | Pets | RLHF Score | Cumulative reinforcement signal that shapes sub-agent behavior |
| **Operant Conditioning Window** | Pets | Feedback Latency | Reinforcement must occur within a time window of the target behavior to register |
| **Tones** | Ambitions | Execution Modes | Configurable behavioral postures during task execution |
| **Active Profession** | Ambitions | Agentic Execution | Real-time, visible, decision-rich task execution (vs. batch processing) |
| **Skill-Based Career** | Ambitions | Freelance Agent | Earning income by directly monetizing capability output |
| **Feat Queue** | Showtime | Execution Plan | Ordered sequence of operations, scored on variety and difficulty |
| **SimFest** | Showtime | Benchmark Competition | Competitive evaluation of agents against each other on the same task |
| **Plasma** | Late Night | Alternative Resource | A non-standard input requirement that replaces the default (e.g., an agent that runs on a different compute substrate) |

---

## III. LORE

Franchise history moments from the Bolte book and guide forewords that illuminate agent design philosophy.

### 1. The Toilet Game as Institutional Resistance Test
The Maxis board of directors called The Sims "the toilet game" and could not believe players would want to simulate chores. EA bought Maxis anyway and greenlit it. **Agent design lesson:** The most transformative agent architectures will face institutional resistance precisely because they don't fit existing categories. "Why would anyone want an AI that just does mundane tasks?" is the toilet game question of 2026.

### 2. Destruction Birthed Creation
Wright made Raid on Bungeling Bay, an action game about destroying factories. He discovered he preferred building the maps to destroying them. The entire Sims franchise descends from a designer who got bored with his own explosions. **Agent design lesson:** The best agent capabilities often emerge from the tools built to support a different purpose. Infrastructure > product.

### 3. Loss as Design Catalyst
In 1991, Wright lost his house to wildfires. Replacing possessions made him question why people buy things to make themselves happy. This existential inquiry became The Sims. **Agent design lesson:** The deepest design insights come from constraint and loss, not from abundance. Build agents that work well under scarcity, not just abundance.

### 4. Language Solved Through Failure Cascade
English dialogue would get repetitive. Real lesser-known languages were too hard for actors. The fallback -- improv gibberish -- accidentally created Simlish, one of gaming's most iconic cultural artifacts. **Agent design lesson:** The best solutions sometimes emerge from failure cascades. When Plan A and Plan B fail, Plan C (the desperate improvisation) can be the breakthrough.

### 5. Forced Multiplayer Failed; Opt-In Sharing Succeeded
The Sims Online (2002) forced multiplayer and died. The Gallery (opt-in sharing of creations) generated 825 million downloads. **Agent design lesson:** Agents sharing outputs voluntarily (via shared knowledge bases, published artifacts) outperforms agents forced into real-time coordination. Async collaboration > forced synchrony.

### 6. Community Corrects the Product
Xmiramira created Melanin Packs because the game lacked realistic dark skin tones. She won Spark'd, and EA subsequently added official skin tone diversity. **Agent design lesson:** Users will extend agent capabilities where the builder fails. Design for extensibility, and treat community contributions as signal, not noise.

---

## IV. EVOLVED INSIGHTS

How the expansions evolved the base game's philosophy in ways relevant to agent design.

### 1. From Optimization to Adaptation (Seasons)
The base game rewards pure optimization: max skills, min time, efficient layouts. Seasons introduced exogenous cycles that cannot be optimized away -- only adapted to. **Agent evolution:** Move from "how do I optimize this agent?" to "how does this agent adapt when its environment changes unpredictably?" Seasonal agents > steady-state agents.

### 2. From Direct Control to Indirect Shaping (Pets)
The base game gives you direct control over Sim actions. Pets introduced entities you shape through reinforcement over time, not command. **Agent evolution:** The RLHF paradigm is Pet training. You cannot tell the model what to do in every situation. You can only Praise and Scold within a feedback window and hope the behavioral meters drift in the right direction. The 2-minute reinforcement window is the most important design constraint in the franchise.

### 3. From Binary Access to Progressive Trust (Visas + Celebrity)
The base game has binary states: you have a skill or you don't, you're friends or you're not. The expansions introduced progressive, earned, revocable access tiers -- Celebrity Levels, Visa Levels, Reputation scores. **Agent evolution:** Agent permissions should be earned progressively, not granted in binary. Level 1 access (read-only). Level 3 access (write). Level 5 access (autonomous action). Each level earned through demonstrated competence, each level revocable through Scandal.

### 4. From Individual to Social Position (Apartment Life)
The base game models individuals. Apartment Life models social stratification -- Class, Group, and Reputation as independent axes of social positioning. **Agent evolution:** An agent's effectiveness depends not just on its individual capabilities but on its position in the social graph of agents. Which group does it belong to? What is its reputation? What class of infrastructure does it occupy? Social position is a stat.

### 5. From Passive Processing to Agentic Execution (Ambitions)
The base game's careers are rabbit-holes: send Sim to work, wait for result. Ambitions made work real-time, visible, and scored. **Agent evolution:** The industry shift from "call an API and wait" to "deploy an agent that works visibly in the world" is exactly the Ambitions shift. Rabbit-hole agents become active profession agents.

### 6. From Competence to Performance (Showtime)
Skills in the base game are private competencies. Showtime made competence public -- evaluated by an audience, scored on variety, penalized for repetition. **Agent evolution:** An agent's capability matters less than its performance quality. Two agents with identical skills will produce different results based on execution planning (feat queue), output diversity (variety scoring), and contextual coherence (stage FX theme matching). Performance is the agent's interface to the world.

### 7. From Fixed Needs to Alternative Architectures (PlantSims, Vampires)
The base game has 6-8 universal needs. PlantSims replaced them with 3 (Sunlight, Water, Love). Vampires replaced Hunger with Thirst. **Agent evolution:** Not all agents need the same resource meters. A research agent might need Data Freshness where a conversation agent needs Social Connectivity. The need system is configurable, not universal. Design agents with custom need profiles, not default ones.

### 8. From Permanent Traits to Irreversible Drift (Werewolf)
The base game's traits are permanent but stable. The Werewolf system permanently rewrites personality toward a fixed archetype (Outgoing 10, Active 10, Playful 10), and curing the condition does NOT undo the drift. **Agent evolution:** Fine-tuning changes the model permanently. You can remove the fine-tuning data, but the model has already drifted. Lycanthropy is catastrophic forgetting, and it is irreversible. Every transformation carries permanent residue.

---

## V. THE CONSTRAINT GRID (EXPANDED)

The base SIB framework defines 10 mutually exclusive trait axes. The expansions add new axes forced by new systems.

| Axis | Pole A | Pole B | Source Expansion | Agent Translation |
|---|---|---|---|---|
| Trust Level | Locked Down | Fully Autonomous | Apartment Life (Alignment) | How much freedom vs. how many guardrails |
| Specialization | Deep (Zone) | Broad (Dabbler) | FreeTime (Enthusiasm) | One domain at Enthusiasm 10 vs. many at 3 |
| Environment | Controlled (Greenhouse) | Wild (Seasonal) | Seasons | Sandbox-buffered vs. exposed to real conditions |
| Control Model | Direct Command | Indirect Shaping | Pets | You tell it what to do vs. you shape it through feedback |
| Execution | Rabbit-Hole (Passive) | Active Profession | Ambitions | Batch processing vs. real-time agentic execution |
| Access | Binary (key or no key) | Progressive (Visa levels) | World Adventures | All-or-nothing vs. earned tiers |
| Output | Private Competence | Public Performance | Showtime | Internal capability vs. scored audience-facing output |
| Resource Model | Standard Needs | Alternative Architecture | Seasons (PlantSim) | Universal meters vs. custom resource profiles |
| Reputation | Anonymous | Celebrity | Late Night | Operating without reputation vs. accumulating social capital |
| Cohabitation | Solo Lot | Shared Apartment | Apartment Life | Isolated runtime vs. multi-tenant shared infrastructure |

---

*Source: Deep dive extractions from 14 expansion pack strategy guides mapped to AI agent architecture.*
*Framework: SIB -- Simulated Intelligence Build*
*Created: 2026-02-20*
