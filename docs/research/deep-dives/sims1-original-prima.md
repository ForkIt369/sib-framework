# Deep Dive: The Sims - Prima's Official Strategy Guide

> **Source:** *The Sims: Prima's Official Strategy Guide* by Mark Cohen
> **Publisher:** Prima Games (2001-2002)
> **Platform:** PC
> **Coverage:** The Sims (base game) + House Party Expansion Pack
> **Pages:** 196

---

## Core Essence

The Sims is a **domestic life simulator** built on interlocking systems of personality, motives, social dynamics, object economics, and career progression. The game has no win state -- it is an open-ended sandbox where player mastery emerges from understanding and manipulating the mathematical relationships between Sim attributes, environmental objects, and social networks. Every object, every interaction, every mood fluctuation is governed by transparent numerical systems that the guide exhaustively documents. The player's role is architect, interior designer, career counselor, social director, and crisis manager for a household of autonomous agents whose behavior follows deterministic rules modulated by personality traits and current motive states.

---

## Key Lexicon

| Term | Definition |
|------|-----------|
| **Motive** | One of 8 internal drives (Hunger, Comfort, Hygiene, Bladder, Energy, Fun, Social, Room) measured on a -100 to +100 scale that collectively determine a Sim's mood and autonomous behavior |
| **Mood Rating** | Weighted average of all 8 motives; physical needs carry more weight when critically low ("Happy Weights" system) |
| **Happy Weights** | Dynamic weighting system where critically low physical motives (below -50) multiply their influence on overall Mood, creating cascading failure states |
| **Motive Engine** | The internal system that calculates Mood from the weighted average of all 8 motive scores |
| **Personality Trait** | One of 5 continuums (Neat/Messy, Outgoing/Shy, Active/Lazy, Playful/Serious, Nice/Grouchy) scored 0-10, drawn from 25 total distributable points |
| **Zodiac Sign** | Astrological archetype that sets default personality point allocation; also governs inter-Sim attraction/repulsion via compatibility matrix |
| **Object Advertising** | System by which objects broadcast motive-fulfillment signals to autonomous Sims; each interaction has an Ad Value, Personality Trait Modifier, and Ad Attenuation (Low/Medium/High) |
| **Ad Attenuation** | Rate at which an object's advertising signal weakens over distance (Low = strong signal far away, High = weak signal far away) |
| **Interaction Queue** | Stack of up to 8 pending actions a Sim will execute in sequence; player-directed or autonomously chosen |
| **Relationship Score** | Asymmetric -100 to +100 value between any two Sims; 50+ = friendship threshold; 70+ = romance potential |
| **Daily Relationship Decay** | Automatic loss of 2 Relationship points per day between Sims who do not interact |
| **Social Outcome Factors** | Variables that modify interaction success: Mood, Relationship Score, Outgoing, Playful, Nice traits, plus contextual flags |
| **Group Talk** | Multi-Sim conversation yielding 8 Social points + 1 Relationship point per speaker turn; restricted to shared conversation topics |
| **Conversation Topic** | One of 12 talk subjects (4 adult-only, 4 kid-only, 4 shared), each with an interest level 1-10; conversations last up to 4 volleys |
| **Fun Type** | Classification of fun activities: Extended (skill-building), One-Time (single burst), Timed (fixed duration), Endless (continuous until interrupted) |
| **Food Chain** | Sequential cooking process: Refrigerator -> Prep Surface (counter/food processor) -> Cooking Appliance; each step adds Hunger satisfaction points |
| **Food Points** | Hunger satisfaction value of a meal, determined by cooking method chain and Sim's Cooking skill level |
| **Purchase Assessment** | Game calculates average value of all household objects; new purchase 20%+ above average = clapping, within 20% = shrug, 20%+ below = wave-off |
| **Object Depreciation** | Every purchasable object has Initial Depreciation (instant loss on placement), Daily Depreciation, and a Depreciation Limit floor |
| **Buyer's Remorse Refund** | 24-hour window after purchase during which objects can be returned for full price |
| **Career Track** | One of 10 job ladders (Entertainer, Law Enforcement, Life of Crime, Medicine, Military, Politics, Pro Athlete, Science, Xtreme, Business) with 10 levels each |
| **Job Performance** | Daily metric determined by Sim's mood when leaving for work; good mood = positive performance, bad mood = negative |
| **Promotion Requirements** | Combination of skill levels and number of Family Friends needed to advance to next career level |
| **Family Friend** | Any Sim with Relationship Score 50+ who lives outside the household; required for career advancement |
| **Major Decision** | Career-specific risk/reward event at certain career levels (Stock Option, The Bribe, Malpractice, etc.) |
| **Chance Card** | Random career event with binary choice; at Level 10, 1-in-20 chance of career track switch |
| **Car Pool** | Daily vehicle that arrives to transport Sim to work; missing the car pool = missed day; 2 missed days = fired |
| **Workday Motive Decay** | Predetermined motive losses during work hours, varying by career track and level |
| **Repo Man** | NPC who repossesses household objects if bills go unpaid for 10 days |
| **Bills** | Arrive in mailbox every 3 days; must be paid within 10 days. Color-coded: White (current), Yellow (3 days overdue), Orange (6 days), Red (9 days) |
| **Grim Reaper** | NPC that appears upon Sim death (starvation or fire); other Sims may plead for the deceased's life |
| **Ghost** | Spirit entity spawning at 11 PM with 1-in-8 chance per urn/tombstone per night; wakes adults, scares awake Sims, won't climb stairs |
| **Tombstone/Urn** | Memorial object placed after Sim death; tombstone if died outdoors, urn if indoors; determines ghost spawn location |
| **Report Card** | Kids' academic grade (A+ through F); drops one letter per bad-mood school day; grade F triggers Military School ($1,000 charge) |
| **Neighborhood** | Self-contained universe of up to 10 lots; Sims from different neighborhoods cannot interact |
| **Party Score** | Numerical rating of House Party event quality, determined by average Mood of all Sims present plus 2 bonus points per guest |
| **Mood Moose** | Visual party indicator: antlers at full extension = high party mood; drooping = poor mood |

---

## The Vibe

Written in a breezy, conversational tone with frequent direct address ("your Sim," "you'll want to...") that masks the mathematical depth underneath. The guide treats the game as a system to be reverse-engineered, with exhaustive data tables presenting every numerical value the game uses internally. Tips from the development team (Andrew Blomquist, Chris Trottier, Peter Trice, Ed O'Tey, Sean Baity) are scattered throughout in callout boxes, providing insider knowledge. The guide oscillates between treating Sims as autonomous agents with their own desires and as optimization targets to be min-maxed. There is a persistent undertone of dark humor -- the guide matter-of-factly discusses killing Sims, walling them in rooms, removing pool ladders, and the mechanics of starvation death, all while maintaining the same clinical analytical voice used for furniture shopping.

---

## New Mechanics Introduced

This is the foundational game, so all mechanics are "new." The guide documents the following systems as the core architecture of The Sims:

### Personality System
- **25 points** distributed across 5 trait continuums (0-10 each)
- **5 Traits:** Neat/Messy, Outgoing/Shy, Active/Lazy, Playful/Serious, Nice/Grouchy
- **12 Zodiac Signs** each with preset personality allocations
- **Zodiac Compatibility Matrix:** determines initial attraction/repulsion between Sims (e.g., Aries attracted to Gemini/Taurus, repelled by Cancer/Virgo)
- Personality directly modifies: autonomous behavior choices, skill-building speed, fun derived from activities, social interaction success rates, TV channel preferences

### Motive System
- **8 Motives** each on -100 to +100 internal scale (displayed as green/red bars)
- **Decay Rates** vary by activity and personality
- **Happy Weights:** Physical motives (Hunger, Bladder, Energy, Hygiene) carry extra weight when critically low
  - Normal weight multiplier at 0 or above
  - Increasing multiplier as motive drops below 0
  - At -100: catastrophic impact on overall Mood
- **Failure States:**
  - Hunger -100 = Death (Grim Reaper appears)
  - Bladder -100 = Accident on floor
  - Energy bottom = Collapse and sleep on floor
  - Comfort/Fun/Social/Room/Hygiene = Mood degradation only (no hard failure)

### Object Advertising System
- Every interactive object broadcasts signals for specific motives
- **Ad Value:** Base motive satisfaction points offered (e.g., Bed advertises Energy 65)
- **Personality Trait Modifier:** Which trait amplifies the object's appeal (e.g., Chess: Serious trait)
- **Ad Attenuation:** How quickly the signal weakens with distance
  - **Low:** Signal reaches far (Sim will cross the lot)
  - **Medium:** Moderate range
  - **High:** Sim must be nearby to notice
- **Interaction Queue Priority:** Autonomous Sims select the highest-value advertisement within range that addresses their most depleted motive
- **False Advertising:** Some interactions promise more than they deliver (noted value vs. actual effect)

### Social Interaction System
- **Relationship Score:** -100 to +100, asymmetric between Sims
- **Interaction Types:** Talk, Joke, Compliment, Entertain, Cheer Up, Brag, Tease, Insult, Scare, Flirt, Hug, Tickle, Dance, Give Gift, Give Backrub, Attack, Kiss, Propose
- **Age Restrictions:** Adult-only interactions (Flirt, Kiss, Give Backrub, Propose, Attack), Kid-only (Tag), Shared (most others)
- **Success/Failure Modifiers:**
  - Current Relationship Score (most influential)
  - Sim's Mood
  - Personality traits (Nice increases positive outcomes, Grouchy increases negative)
  - Outgoing trait affects romantic interaction success
- **Conversation System:**
  - 12 topics (4 adult: Money, Weather, Politics, '60s Stuff; 4 kid: Toys, Sports, Aliens, Pets; 4 shared: Outdoors, Travel, Music, Food)
  - Each Sim has interest levels 1-10 per topic
  - Matching high interests = positive volleys; mismatched = negative
  - Up to 4 volleys per conversation
  - Group Talk uses only shared topics (4 of 12)
- **Relationship Decay:** 2 points/day for all non-household relationships
- **Friendship Threshold:** 50+ Relationship Score
- **Romance Threshold:** 70+ Relationship Score, plus sufficient positive romantic interactions

### Career System
- **10 Career Tracks** with 10 levels each:
  1. Entertainer ($100/day at Level 1 -> $1,400/day at Level 10)
  2. Law Enforcement ($240 -> $1,200)
  3. Life of Crime ($200 -> $1,400)
  4. Medicine ($200 -> $1,500)
  5. Military ($250 -> $1,500)
  6. Politics ($220 -> $1,400)
  7. Pro Athlete ($110 -> $1,300)
  8. Science ($155 -> $1,400)
  9. Xtreme ($175 -> $1,325)
  10. Business ($120 -> $1,200)
- **6 Skills:** Cooking, Mechanical, Charisma, Body, Logic, Creativity (each 0-10)
- **Skill Building Methods:**
  - Cooking: Bookshelf (Study Cooking)
  - Mechanical: Bookshelf (Study Mechanical) or repair broken objects
  - Charisma: Mirror or Medicine Cabinet (Practice Speech)
  - Body: Exercise Machine, Pool, Basketball Hoop
  - Logic: Chess Set, Telescope
  - Creativity: Easel (Painting), Piano
- **Personality-to-Skill Speed Modifiers:**
  - Active Sims build Body faster
  - Serious Sims build Logic faster
  - Outgoing Sims build Charisma faster
  - Playful Sims build Creativity faster
- **Career-to-Personality Matching:** Table maps ideal personality configurations per career based on required skill mix
- **Job Finding:** Newspaper (1 listing/day, delivered daily) or Computer (3 listings/day)
- **Car Pool timing** varies by career level and hours

### Economic System (Sim Economics 101)
- **Bills:** Arrive every 3 days based on total household object value
- **Bill Escalation:** White -> Yellow (3 days) -> Orange (6 days) -> Red (9 days) -> Repo Man (10 days)
- **Repo Man:** Repossesses items equal to unpaid bill value
- **Object Depreciation:** Every object loses value from purchase moment
  - Initial Depreciation: Immediate loss on placement (varies by object)
  - Daily Depreciation: Ongoing loss per Sim-day
  - Depreciation Limit: Minimum resale value floor
- **Income Sources:** Career salary, selling paintings (value = average skill level of painters * $50), Slot Machine (if Casino object available)
- **Services with Costs:**
  - Maid: $10/visit (auto-scheduled or phone)
  - Gardener: automatic lawn care
  - Repairman: $50/hour
  - Pizza Delivery: $40/pizza
  - Firefighter: automatic on fire alarm
  - Police: automatic on burglar alarm

### Building System
- **Terrain Tools:** Raise/Lower terrain, Level Terrain
- **Wall Tool:** Interior ($35/section) and Exterior ($70/section), Diagonal walls
- **Door Tool:** 5 models ($100-$400), privacy/bathroom considerations
- **Window Tool:** 8 models ($55-$200), affect Room motive and lighting
- **Floor Covering:** Paint/remove tiles
- **Wallpaper Tool:** Interior/exterior surfaces
- **Staircase:** $900, single model, requires specific space
- **Roof Tool:** Shallow/Medium/Steep pitch, 4 patterns
- **Water Tools:** Pool ($75/tile), Diving Board ($300), Ladder ($200), Decking
- **Fireplace Tool:** 4 models ($600-$3,000)
- **Plant Tool:** 14 plants (Flowers 4, Bushes 1, Hedges 2, Shrubs 2, Trees 5)
- **Key Building Principles:**
  - 2-square-wide hallways minimum to prevent pathing bottlenecks
  - Double doors at high-traffic points
  - Privacy for bathrooms (separate rooms with doors)
  - Room size affects Room motive score
  - Windows boost Room score and provide light
  - Corner rooms round off counters automatically

### Family & Life Events
- **Marriage:** Requires Relationship 70+ and sufficient romantic interaction history; Propose option appears; spouse moves in with their job and bank account
- **Babies:** Passionate Kiss has 1-in-5 pregnancy chance; also Adoption phone call random event; Love Bed has 1-in-8 chance
- **Baby Care:** Feed and interact when crying; neglect triggers Social Worker who permanently removes child
- **Kids:** Attend school 8am-3pm, Report Card grades, can study on bookshelf, cannot use adult-only objects
- **Death:** Starvation (Hunger -100), Fire (adjacent combustible tile), Electrocution (repairing electronics based on Mechanical skill), Drowning (pool with no ladder)
- **TV Repair Hazard Table:**
  - Mechanical 0: 100% electrocution chance
  - Mechanical 1: 25%
  - Mechanical 2: 10%
  - Mechanical 3-10: 1%

### Fire, Theft, and Accidents
- **Fire:** Can start from Stove (low Cooking skill), Fireplace (adjacent combustible), or random
- **Burglar:** Random nighttime event; Burglar Alarm ($250) auto-calls police; alarm detects motion within 5 exterior grid tiles
- **Roaches:** Appear from dirty objects/food left out; exterminate by having Sim stomp them
- **Floods:** From broken plumbing (Sink, Dishwasher, Bathtub, Shower); Repair skill determines fix speed

### Ghost Mechanics
- **Spawn Time:** 11 PM
- **Spawn Chance:** 1-in-8 per urn/tombstone per night
- **Behavior:** Wakes sleeping adults (not kids), scares awake Sims, won't climb stairs
- **Removal:** Sell the urn/tombstone; ghost permanently disappears
- **Mourn Interaction:** Tombstone/urn advertises Mourn interaction very highly for first 24 Sim-hours, then decreases over 48 more hours

---

## Systems & Architecture

### The Motive-Mood-Behavior Loop
The central gameplay loop: Motives decay over time -> Mood degrades -> Autonomous Sim seeks objects advertising relevant motive relief -> Interaction satisfies motive -> Mood improves -> Cycle repeats. Player intervention disrupts this loop by directing Sims to specific interactions that may not be the highest-advertised option but serve longer-term goals (career advancement, relationship building). The tension between autonomous self-preservation and player-directed strategic goals is the core gameplay dynamic.

### Object Ecosystem
Every purchasable object exists within a web of relationships:
- **Motive Fulfillment:** Which needs it addresses and how effectively
- **Skill Building:** Whether it builds career-relevant skills
- **Social Facilitation:** Whether it enables group activities (hot tub, chess, TV, pool table, piano)
- **Room Score Impact:** Decorative value (positive or negative)
- **Economic Value:** Purchase price, depreciation rate, and resale trajectory
- **Breakability:** Whether it can malfunction, flood, or cause fire
- **Space Requirements:** Physical footprint and placement constraints

### Complete Object Interaction Catalog (Chapter 9)
The guide provides an A-to-Z catalog of every object with:
- Cost range
- Motives affected
- Group activity status
- Breakable/unbreakable
- Adult-only/kid-only restrictions
- Behavioral notes

Key objects and their unique properties:
- **Aquarium ($200):** Fun motive, gets dirty if not cleaned, fish die if not fed
- **Bar ($780-$800):** Fun, Hunger, Bladder (lowers); adults make drinks, kids get soda
- **Barbecue ($350):** Hunger, group meal; can start fires on adjacent tiles
- **Basketball Hoop ($650):** Fun, Energy (lowers); Body skill; Active trait modifier
- **Bookshelf ($250-$910):** Fun, Cooking/Mechanical/Study skills; Serious Sims autonomously read for Fun
- **Chess Set ($500):** Fun, Logic skill; group activity; Serious trait = more Fun
- **Computer ($999-$6,500):** Fun, Get Job, Study (kids); cheaper = breaks sooner
- **Easel ($3,500):** Fun, Creativity skill; paintings sellable (skill 0 = $0, skill 5 = $25, skill 10 = $500)
- **Fireplace ($600-$3,000):** Burns 2 hours, Room score; anything combustible on adjacent tile catches fire
- **Grandfather Clock ($3,500):** Room motive, runs 24 hours per winding
- **Hot Tub ($6,500):** Comfort, Fun, Hygiene; group activity; Outgoing 7+ = naked entry
- **Piano ($3,500-$5,399):** Fun, Creativity skill; advertises "Come and See Me" to visitors; high Creativity = better music quality
- **Pool Table ($4,200):** Fun; group activity; high Fun boost
- **Tombstone/Urn:** Mourn interaction; ghost generation; Social motive lowering effect on nearby Sims
- **Train Set ($955):** Fun; group activity for up to 10 Sims; observer Fun increases with more participants
- **Voodoo Doll:** Shakes, slaps, or sticks pins into target Sim (appears in PIP window); if target is in room, they approach and slap user

### Visitor Autonomous Activities Table
When visitors arrive, they autonomously seek activities based on personality:
- **Active visitors** gravitate toward physical objects (exercise, basketball, pool)
- **Lazy visitors** prefer sedentary options (TV, couches, hot tub)
- **Outgoing visitors** seek social objects (phone, group activities)
- **Nice visitors** help with household chores
- **Grouchy visitors** may autonomously insult or pick fights

### The Party Score System (House Party)
- Score = average Mood of all Sims present + 2 per non-resident guest
- Score ranges from -100 to +100
- Tallied every 20 game-minutes
- **Fleeting Fun mechanic:** While party is active, all Sims lose Fun at 2x normal rate every 5 game-minutes (forcing active entertainment management)
- **NPC Triggers:**
  - **Psycho Mime:** Appears at 90+ game-minutes if party score is 15 or below; also at all-family parties (5+ family members + Caterer)
  - **Party Crashers:** Appear at 120+ game-minutes if score is 40+; live in neighborhood; may sleep over
  - **Secret Celebrity:** Appears at 135+ game-minutes if score is 55+; stays max 4 hours; leaves if score drops below 45
- **Police:** Break up party if it runs past 11 PM

---

## House Party Expansion

### New Systems
- **Party Themes:** Western, Luau, Rave -- each with matched furniture sets, wall/floor textures, and costume trunk options
- **Costume Trunk ($496):** Group activity; everyone at party changes to selected theme outfit
- **Equipment Rental:** Buy party objects within 24 hours, sell back at full price after party (essentially free rental)
- **Caterer ($350/24 hours):** Stocks buffet tables, makes punch; requires at least one Buffet Table; sociable with guests
- **Entertainer:** Hired via Fancy Feet Cake Treat ($300); male or female dancer; entertains and socializes with guests
- **Campfire Ghost:** 1-in-10 chance when adult Sim (Charisma 6+) selects Tell Story at KampRite Instant Campfire

### New Objects (50+ items)
- **Seating:** Freedom Chair ($65), Rusty Redneck Barrel Chair ($100), Inflatable Fun Chair ($109), Surplus Theatre Seating ($153), Tiki Dream Dining Chair ($600), Chair of the Future ($203), Tropi-Cane Island Chair ($315), Cowch Country Lounger ($1,115)
- **Couches:** Inflatable Sofa ($190), Tropi-Cane Sofa ($535), Cowch Country Sofa ($1,350)
- **Surfaces:** Smart Counter ($432), Cape Crab Coastside Counter ($249), Country Counter ($276), ScienStone Wall Counter ($425), Freedom End Table ($40), Elegant Chef End Table ($50), "Lola Mona" Occasional Table ($170), Efficiency Table ($179), Efficiency Table Plus! ($275), Artist's Concept Table ($349), Tiki Dream Dining Table ($379)
- **Decorative:** Party Balloons ($50, pop within a day), Desert Nut Lawn Ornament ($70), "Amaizing" Lawn Ornament ($89), Jungle Jumble Import Display ($151), Pacific Island Relic ($198), "Duke Tubula" Memorial Surf Board ($230), Scraps Ranch Rag Rug ($233), Davant-Naif Art Rug ($290), Long Horn Wall Accent ($395), Beaver Pelt Moosehead ($450), Weft Wrights Wall Quilt ($515), "Black Bile Bear" ($520), "Native Sim Wall Hanging" ($639), SimBad's Stuffed Marlin ($777), "Blue Inca Pilot" Band Poster ($1,789), Ali'i Kahuna Ceremonial Tiki ($2,000)
- **Electronics/Dance Aids:** "Bounce My Booty" Dance Floor ($1,250, Fun 6, Room 2), Spazmatronic Plasmatronic Go-Go Cage ($1,749, Fun 7, Room 3; group activity + dance), Neukum Stereo Speakers ($99), Turntablitz DJ Booth ($7,129, Fun 8, Room 3; ultimate sound system, Playful Sims can scratch), ToroTec Mechanical Bull ($5,678, Fun 4, Body skill; difficulty setting affects payout)
- **Plumbing:** Boggs Memorial Commode ($375, Bladder 8), Chrome Faucet System ($622, Hygiene 3), Wicked Breeze Surf Shower ($672, Hygiene 5, Room 1)
- **Lighting:** Faux Blowfish Fish Lamp ($173), Club Code Thrill Light ($1,000, Room 1), SUNOT Shop Light ($30), Old Railroad Lamp ($63), LED Pod Light ($131), Symbol Light ($135)
- **Miscellaneous:** Ornery Owl Pioneer Bookcase ($935, Cooking/Mechanical/Study), Galvanator Bookshelf ($925, Cooking/Mechanical/Study), Whether Vain Drink Dispenser ($920, Hunger 1, Fun 3, Room 3), Antique Saloon Drink Cabinet ($922, Hunger 1, Fun 3, Room 3), Punchucopia Extraordinaria ($150, group punch bowl), Elegant Chef Buffet Table ($194, Hunger 4, requires Caterer), Fancy Feet Cake Treat ($300, Fun 3, summons Entertainer), KampRite Instant Campfire ($482, Comfort 2, Fun 2; Charisma 6+ = ghost chance), "Bezique's Folly" Card Game ($502, Fun 2, Charisma skill), Super Schlooper Bubble Blower ($710, Comfort 2, Fun 3; group activity up to 4), Porta-Parody Costume Trunk ($496, group activity, theme costumes)

### House Party Object Advertising Table
Complete table for all new objects with columns:
- Object Type | Possible Interactions | Motive Advertised | Advertised Value | Personality Trait Modifier | Reduced Effects (Over Distance)

Key entries:
- DJ Booth: Turn Off (Energy 220, Neat, Medium), Turn On/Dance/DJ (Fun 30-65, Playful/Outgoing/Creativity), Watch (Fun 40, Shy, High)
- Mechanical Bull: Ride (Fun 45, Active, Medium), Watch (Social 40, N/A, High)
- Dance Floor: Dance (Fun 60, Active, High), Join (Social 70, N/A, High)
- Buffet Table: Grab a Plate (Hunger 95, N/A, Low)
- Campfire: Sit (Fun 42, Charisma, Medium), Join (Fun 42 + Social 60, N/A, Medium)

### House Party NPCs
- **Campfire Ghost:** Rare sighting from campfire storytelling (1-in-10 chance, Charisma 6+ required)
- **Caterer:** Hired for $350/24 hours, stocks buffet tables, sociable, hits on guests when idle
- **Entertainer:** Summoned via Fancy Feet Cake Treat, boosts Mood via dance show, socializes after
- **Psycho Mime:** Kleptomaniac who steals food and small items from countertops (except Bezique's Folly set); appears at low-scoring or all-family parties; actually helps party mood despite thievery
- **Party Crashers:** Random well-behaved strangers who boost party score; appear at 120+ minutes if score 40+
- **Secret Celebrity:** Mystery VIP guest at 135+ minutes if score 55+; stays max 4 hours; leaves if score drops below 45

### New Neighborhoods
- House Party adds 3 new neighborhoods (10 lots each) to the existing 5 (original) + 4 (Livin' Large) = grand total of 12 neighborhoods (120 lots)
- Each neighborhood is an isolated universe
- Warning: Installing House Party after Livin' Large may affect neighborhoods 2-5

### Party Timeline Checklist
- 9:00 AM: Best Cook makes breakfast
- 10:00 AM: Group fun activity
- 11:00 AM: Bathrooms/hygiene
- 12:00 PM: Nap time; buy party objects while Sims sleep
- 4:00 PM: Wake up, urgent needs, call Caterer
- 5:00 PM: First invite call
- 5:30 PM: Party begins
- 6:00 PM: First guests should be eating
- 6:30 PM: Second invite call
- 7:30 PM: Hire Entertainer
- 8:00 PM: Monitor mood, dismiss unhappy guests
- 10:00 PM: Start dismissing guests (police come at 11 PM)

---

## Modding & Customization (Chapter 10)

### Mesh vs. Skin
- **Mesh:** 3D wireframe shape of a Sim's body/head
- **Skin:** Colored texture wrapped around the mesh
- Cannot edit meshes in-game; can create/swap skins

### Official Tools
- **FaceLift:** Free utility for creating new Sim heads by morphing preset shapes; exports directly to game folder
- **HomeCrafter:** Preview and import custom floor/wall textures; loads .bmp/.jpg files; wall and floor tiles can be priced as low as $1 (decorating cost cheat)
- **SimShow:** Preview body/head skins and animations; export to game folders
- **SimTransmogrifier:** Clone existing objects, edit catalog text/description/price, modify graphics

### File Locations
- Head/body textures: `The Sims\GameData\Skins`
- Floors: `The Sims\GameData\Floors`
- Walls: `The Sims\GameData\Walls`
- Roofs: `The Sims\GameData\Roofs`
- Roof patterns: 256-color .bmp, 32x32 pixels, 8-bit depth

### MP3 Music Integration
- Custom music in `Music\Stations\[Country|Classica|Latin|Rock]`
- Build Mode music: `Music\Modes\Build`
- Buy Mode music: `Music\Modes\Buy`
- Neighborhood music: `Music\Modes\NhoodUS`

### Sharing Families
- Export HTML family pages via Play Options
- Family .jpg files saved in `Web Pages` folder
- Upload to The Sims Exchange for community sharing
- Import families via `UserData\Import` folder
- Families are lot-specific: must match lot number in destination neighborhood

---

## Core Insight

The Sims is not a life simulator -- it is an **economics engine** where the currency is *time* and the commodity is *satisfaction*. Every system in the game reduces to a resource allocation problem: 24 Sim-hours per day must be distributed across 8 competing motives, skill development, social maintenance, career obligations, and environmental management. The genius of the design is that motives decay at different rates and carry different weights, creating a perpetual juggling act where optimal play means accepting strategic dissatisfaction in low-priority areas to invest in high-return activities. The personality system does not create "characters" so much as it creates different *optimization curves* -- a Neat Sim and a Messy Sim are not narratively different; they are mathematically different in terms of which objects advertise most effectively to them and which skills they build fastest. The entire game is, at its core, a scheduling problem with stochastic social disruptions.
