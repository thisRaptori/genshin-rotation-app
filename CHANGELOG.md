# 7.1.2

- Added **Browse**: submit and share rotations with the community, and vote on others'
- Added **Practice**: an in-browser rhythm-game mode that scores you against a rotation's timeline
- Added an animated intro banner walking new users through Browse, Build, Practice, and Share

# 7.1.1

- Added Zibai frames

# 7.1.0

- Added beta Vesna and Vodyanitsa
- Added rotation stats
  - Total rotation duration
  - Exact on-field time per character
  - Energy gained per character (particles & flat energy)
  - Upper bound ER requirement per character
- Added 7.1 weapons
  - 5 Star
    - Catalyst
      - Hymn of the Maelstrom
    - Sword
      - Beyond the Chrysalis
  - 4 Star
    - Bow
      - Breezeborne Refrain
    - Catalyst
      - Winter's Heavy Heart
    - Sword
      - New Bough
      - Silver Light

# 7.0.0

Finished the v2 implementation! It's currently up to date with everything including the new characters released in 7.0; read below to see the full audit of what was implemented when.

There will likely be a lot of issues to iron out, but overall it's significantly more accurate than before. The main difference is that instead of rough estimates based on best guesses, the app actually models the real logic behind systems like auras, gauge theory, reactions, etc, so frame-perfect timing is now possible to achieve!

Thanks again to Sylv (tahubezdachu) for helping test things!

# v2 ground-up re-implementation

Added beta v2 implementation! Beta updates will be logged in the in-app updates page, and this changelog will only become active again once the beta is complete and the old implementaion is removed.

## Beta updates

The following were logged in the in-app v2 updates page over the course of the beta:

### 10th September 2026

- Added Prune, Sandrone, Odette, Alyosha, and Cryo Traveler
- Added meter indicators to Varesa, Kachina, Kinich, Mualani, Mavuika, Ifa, Iansan, Ororon, Pyro Traveler, and Freminet
- Implemented missing Hexerei and Revelations buffs
- Added nightsoul dash/jump mechanics to Iansan and Varesa
- Rewrote rotation → gcsim output generator

### 7th September 2026

- Added Durin, Jahoda, Columbina Hyposelenia, Zibai, Illuga, Varka, Linnea, Nicole, and Lohen
- Added optional meter indicators to Lohen, Zibai, Skirk, and Xilonen (more coming soon!)
- Fixed some character hitmarks for multi-hit attacks
- Fixed Flins frames and hitlag extensibility

### 5th September 2026

Back from a bit of a break with several new characters and a ton of cleanup work:

- Added Skirk, Ifa, Dahlia, Ineffa, Lauma, Aino, Flins, and Nefer
- Added Lunar reactions, Moonsign tracking, Verdant Dew, Seeds of Deceit, and Stellar Conduct
- Ran an accuracy audit-and-fix pass against gcsim and the official wiki for every existing character, correcting frame timings, hitmark counts, cooldowns, energy/particle generation, buff durations, and constellation/passive behaviour that had drifted from their real kits
- Added artifact sets:
  - A Day Carved from Rising Winds
  - Aubade of Morningstar and Moon
  - Celestial Gift
  - Disenchantment in Deep Shadow
  - Finale of the Deep Galleries
  - Heart of the Furnace
  - Long Night's Oath
  - Night of the Sky's Unveiling
  - Scarlet Proof
  - Silken Moon's Serenade
- Fixed and expanded existing artifact sets:
  - Celestial Gift
  - Crimson Witch of Flames
  - Flower of Paradise Lost
  - Golden Troupe
  - Husk of Opulent Dreams
  - Nymph's Dream
  - Obsidian Codex
  - Scholar
  - Scroll of the Hero of Cinder City
  - Shimenawa's Reminiscence
  - Silken Moon's Serenade
  - Song of Days Past
  - The Exile
  - Thundering Fury
  - Vermillion Hereafter
- Fully implemented a large batch of weapons across every type:
  - Bows: Astral Vulture's Crimson Plumage, Covenant of Frost and Snow, Flower-Wreathed Feathers, Golden Frostbound Oath, Hunter's Path, Ibis Piercer, King's Squire, Messenger, Mitternachts Waltz, Polar Star, Predator, Prototype Crescent, Rainbow Serpent's Rain Bow, Range Gauge, Scion of the Blazing Sun, Sequence of Solitude, Silvershower Heartstrings, Skyward Harp, Snare Hook, Song of Stillness, The Daybreak Chronicles, The Viridescent Hunt, Thundering Pulse, Windblume Ode
  - Catalysts: Ash-Graven Drinking Horn, Clash of Kings, Dawning Frost, Echoes of the Heart, Etherlight Spindlelute, Hakushin Ring, Jadefall's Splendor, Kagura's Verity, Lost Prayer to the Sacred Winds, Mappa Mare, Memory of Dust, Nightweaver's Looking Glass, Nocturne's Curtain Call, Oathsworn Eye, Otherworldly Story, Prototype Amber, Reliquary of Truth, Ring of Yaxche, Sacrificial Jade, Skyward Atlas, Solar Pearl, Sunny Morning Sleep-In, Surf's Up, The Widsith, Thrilling Tales of Dragon Slayers, Tome of the Eternal Flow, Tulaytullah's Remembrance, Vivid Notions, Waveriding Whirl, Wine and Song
  - Claymores: A Teaspoon of Transcendence, A Thousand Blazing Suns, Blade of Atonement, Earth Shaker, Fang of the Mountain King, Flame-Forged Insight, Fruitful Hook, Gest of the Mighty Wolf, Katsuragikiri Nagamasa, Luxurious Sea-Lord, Mailed Flower, Master Key, Portable Power Saw, Prototype Archaic, Serpent Spine, Skyrider Greatsword, Skyward Pride, Snow-Tombed Starsilver, Song of Broken Pines, The Bell, The Unforged, Tidal Shadow, Verdict, Whiteblind
  - Polearms: Bloodsoaked Ruins, Disaster and Remorse, Footprint of the Rainbow, Fractured Halo, Frostbreath, Halberd, Kitain Cross Spear, Lumidouce Elegy, Missive Windspear, Moonpiercer, Mountain-Bracing Bolt, Primordial Jade Winged-Spear, Prospector's Drill, Prototype Starglitter, Rightful Reward, Sacrificer's Staff, Skyward Spine, Song of the Vigil, Staff of the Scarlet Sands, Symphonist of Scents, Tamayuratei no Ohanashi, Vortex Vanquisher
  - Swords: Athame Artis, Azurelight, Emberwell, Exaiphanes Blade, Flute of Ezpitzal, Haran Geppaku Futsu, Heretic's Molten Blade, Iron Sting, Kagotsurube Isshin, Key of Khaj-Nisut, Light of Foliar Incision, Lightbearing Moonshard, Mistsplitter Reforged, Peak Patrol Song, Prototype Rancour, Sapwood Blade, Serenity's Call, Skyrider Sword, Skyward Blade, Splendor of Tranquil Waters, Sturdy Bone, Summit Shaper, Sword of Descension, Sword of Narzissenkreuz, The Dockhand's Assistant, The Flute, Traveler's Handy Sword, Uraku Misugiri, Whitelake Frostfeather, Wolf-Fang
- Fixed and expanded existing weapons:
  - Amenoma Kageuchi
  - Cashflow Supervision
  - Crane's Echoing Call
  - Dark Iron Sword
  - Dialogues of the Desert Sages
  - Emerald Orb
  - Everlasting Moonglow
  - Fading Twilight
  - Fleuve Cendre Ferryman
  - Forest Regalia
  - Fruit of Fulfillment
  - Sacrificial Greatsword

### 12th January 2026

- Added Escoffier

### 7th January 2026

- Added Iansan
- Added more weapons: Fleuve Cendre Ferryman, Flowing Purity, Freedom Sworn, Frosbearer, Fruit of Fulfillment
- Added rough movement estimates to all existing character actions
- Fixed Diluc and Klee chain interruptions
- Added icons for Keqing and Diluc skill recast
- Fixed various bugs in Keqing's implementation

### 2nd January 2026

- Added Hexerei buffs for existing characters (Albedo, Fischl, Klee, Mona, Razor, Sucrose, and Venti)
- Fixed various bugs in the hexerei characters
- Fixed claymore charged hit counts
- Fixed various issues in Qiqi's implementation

### 2nd December 2025

- Added Varesa
- Fixed Jean burst healing timing, enter/exit damage, and C2 implementation
- Fixed Obsidian codex detection for several characters
- Removed ICD from Anemo traveler storm hit
- Removed ICD from Aether plunge
- Implemented geo construct limit
- Fixed Albedo construct creation
- Fixed Geo traveler burst construct creation timing

### 22nd November 2025

- Added Mizuki
- Added more weapons: Emerald Orb, Engulfing Lightning, Everlasting Moonglow, Eye of Perception, Fillet Blade, Finale of the Deep
- Fixed infusion durations and added more extensive logging
- Fixed Chongyun C1
- Fixed Bennett C4
- Fixed Noelle normal cancels and burst infusion
- Fixed Sigewinne bond calculation

### 18th November 2025

- Added Pyro Traveller
- Fixed Xingqiu and Beidou coordinated attack trigger conditions
- Added Ningguang A4 passive support on dash

### 15th November 2025

- Added Mavuika, Citlali, and Lanyan
- Added more weapons: Dialogues of the Desert Sages, Dodoco Tales, Dragonspine Spear
- Fixed Xingqiu's burst
- Fixed dash infusions

### 12th November 2025

- Added characters up to 5.2 (Xilonen, Chasca, and Ororon)
- Added more weapons: Crane's Echoing Call, Crescent Pike, Crimson Moon's Semblance, Dark Iron Sword, Debate Club
- Added missing hitlag extension for various Fontaine characters
- Added Lyney C2
- Added Sigewinne C6
- Fixed Navia's infusion/plunge interaction

### 8th November 2025

- Added characters up to 5.0 (Kachina, Kinich, Mualani)
- Added Nightsoul Blessing and Nightsoul Bursts
- Added Cinder City and Obsidian Codex artifact sets
- Added more weapons: Absolution, Amenoma Kageuchi, Ballad of the Boundless Blue, Beacon of the Reed Sea, Bloodtainted Greatsword, Calamity Queller, Cashflow Supervision

### 5th November 2025

- Added characters up to 4.8 (Sigewinne and Emilie)
- Started adding weapons: Alley Hunter, Cloudforged, Compound Bow, Elegy for the End, End of the Line, Fading Twilight, Favonius (Codex, Greatsword, Lance, Sword, and Warbow), Sacrificial (Bow, Fragments, Greatsword, and Sword)
- Fixed Arlecchino skill cooldown
- Added Gorou's burst crystallise shard consumption
- Fixed Clorinde's A1 passive
- Fixed Amber's C2, C4, and burst tick count
- Fixed Xiangling C1 and burst ICD, and added guoba swirl mechanic to Sucrose's skill

### 2nd November 2025

- Added Arlecchino, Clorinde, and Sethos
- Added Bond of Life mechanics
- Added Fragment of Harmonic Whimsy artifact set

### 28th October 2025

- Added characters up to 4.5 (Xinyan, Gaming, Chiori)
- Fixed Sucrose A1 overlap
- Consolidated plunge attacks and corrected some incorrect frames
- Added constructs system

### 25th October 2025

- Added characters up to 4.3 (Freminet, Neuvillette, Wriothesley, Furina, Charlotte, Navia, and Chevreuse)
- Updated the character sort order to match the in-game order
- Adjusted Xiangling's chili pepper mechanic - you now need to dash to pick it up!
- Added crystallise shard tracking - also requires a dash to pick up shards

### 22nd October 2025

- Added most of the characters from 4.0 (Hydro Traveler, Lyney, and Lynette)
- Connected v2 to account-level character constellation/weapon/artifact setup
- Fixed Dehya's skill/burst interaction
- Fixed Baizhu C6
- Added Diona charged attack ICD
- Reset jump height before switching characters
- Added persistent updraft after Venti hold skill (allows plunge attack after jump)
- Fixed Barbara's C4 and charged attack ICD
- Fixed Kaeya's A4 Passive and ICDs
- Fixed Mika's attack speed buff
- Rewrote the damage and elemental application system to enable Shatter and improve accuracy

### 18th October 2025

- Added characters up to 3.7 (Layla, Wanderer, Yaoyao, Dehya, Mika, Baizhu, Kaveh, and Kirara)
- Fixed Xingqiu's C2
- Fixed Klee's burst duration

### 15th October 2025

- Added characters up to 3.1 (Dendro Traveler, Collei, Tighnari, Dori, Cyno, Candace, and Nilou)

### 12th October 2025

- Added characters up to 2.8 (Ayato, Yelan, Kuki, and Heizou)
- Added hitlag extension for elemental auras

### 8th October 2025

- Added characters up to 2.5 (Thoma, Itto, Gorou, Shenhe, Yun Jin, and Yae Miko)
- Added hitlag extension support (note: aura extension is also done)
- Added some tweaks to the app's layout to better support different screen sizes!

### 5th October 2025

- Added characters from 2.0 and 2.1 (Electro Traveler, Ayaka, Sayu, Yoimiya, Sara, Raiden, and Kokomi)

### 2nd October 2025

We finally have the absolute basics of the rewrite up and running!

In order to accurately represent more complex characters, we've started from scratch, using a completely different approach which lets us include more technical details like ICDs and gauge theory.

Note that this is a very early version, and since every single feature has a lot of nuances which only become apparent when used together with all the _other_ features, there were many inaccuracies at this stage.

# 4.7.2

- Fixed Noelle infusion on swap

# 4.7.1

- Added Clorinde frames

# 4.7.0

- Added Clorinde
- Added Sethos
- Added Sigewinne
- Added 4.5 Artifact sets
  - Fragment Of Harmonic Whimsy
  - Unfinished Reverie
- Added 4.7 Weapons
  - 5 Star
    - Bow
      - Silvershower Heartstrings
    - Sword
      - Absolution
  - 4 Star
    - Bow
      - Cloudforged

# 4.6.2

- Added Arlecchino C4

# 4.6.1

- Added Arlecchino frames

# 4.6.0

- Added beta Arlecchino
- Added 4.6 weapon
  - 5 Star
    - Polearm
      - Crimson Moon's Semblance

# 4.5.0

- Added Chiori
- Gaming frames
- Added 4.5 weapons
  - 5 Star
    - Sword
      - Uraku Misugiri
  - 4 Star
    - Polearm
      - Dialogues of the Desert Sages

# 4.4.0

- Added `window.genshinRotation` property to allow users to customise values
- Added beta Xianyun
- Added beta Gaming
- Added 4.4 weapon
  - 5 Star
    - Catalyst
      - Crane's Echoing Call

# 4.3.3

- Chevreuse frames
- Added hold option for Ayato's charged attack

# 4.3.2

- Added beta Chevreuse
- Added 4.3 second half weapons
  - 4 Star
    - Claymore
      - Ultimate Overlord's Mega Magic Sword

# 4.3.1

- Navia frames
- Charlotte frames
- Wriothesley frames
- Remove action latency after burst swap
- Disabled yelan skill swap cancel

# 4.3.0

- Added beta Navia
- Added Artifact Sets
  - Nighttime Whispers in the Echoing Woods
  - Song of Days Past
- Added 4.3 first half weapons
  - 5 Star
    - Claymore
      - Verdict

# 4.2.1

- Furina frames
- Furina C6 - added 6-hit limit to infusion

# 4.2.0

- Added beta Furina
- Added beta Charlotte
- Added 4.2 weapons
  - 5 star
    - Sword
      - Splendor of Tranquil Waters
  - 4 star
    - Sword
      - Sword of Narzissenkreuz
- Fixed visual bug for charged actions shorter than 48 frames

# 4.1.3

- Added beta Wriothesley
- Added 4.1 second half weapons
  - 5 star
    - Catalyst
      - Cashflow Supervision
  - 4 star
    - Bow
      - Range Gauge
    - Polearm
      - Prospector's Drill

# 4.1.2

- Re-adjust Neuvillette frames
- Fix charged attack details and drag position

# 4.1.1

- Neuvillette frames
- Added 4.1 first half weapons
  - 5 star
    - Catalyst
      - Tome of the Eternal Flow
  - 4 star
    - Catalyst
      - Ballad of the Boundless Blue
    - Claymore
      - Portable Power Saw
    - Sword
      - The Dockhand's Assistant

# 4.1.0

- Added beta Neuvillette

# 4.0.9

- Freminet frames & normals implementation (does not include burst mechanics)
- Added Kazuha elemental damage buff duration display

# 4.0.8

- Added charged attack visual indicator
- Enabled constellation-specific frames and hitmarks
- Added Ganyu C6
- Added Tighnari C6
- Added Faruzan C1

# 4.0.7

- Fix Dori infusion
- Fix Razor cooldowns
- Added Diona C4

# 4.0.6

- Added Lynette C4
- Removed duration from Wanderer burst

# 4.0.5

- Added Jean hold skill variant
- Heizou & Jean n -> c frames fix
  - A couple of frames were set to 500 since that's how gcsim approached them, no idea why they did that, so just removing.

# 4.0.4

- Lyney frames
- Lynette frames

# 4.0.3

- Fix end on swap in some situations
  - e.g. when character receiving buff doesn't go off-field at tend of rotation
- Add sucrose swirl duration to all attacks

# 4.0.2

- Fixed Dehya C2 & C6 skill extensions
- Fixed Nahida C5

# 4.0.1

- Fixed Kazuha plunge attack infusion priority
- Fixed UI for editing account characters

# 4.0.0

- Added 4.0 characters
  - Lyney
  - Lynette
  - Freminet
- Added 4.0 artifact sets
  - Golden Troupe
  - Marechaussee Hunter
- Added 4.0 weapons
  - 5 star
    - Bow
      - The First Great Magic
  - 4 star
    - Bow
      - Scion of the Blazing Sun
      - Song of Stillness
    - Catalyst
      - Flowing Purity _(note: only initial simple passive implemented)_
      - Sacrificial Jade _(note: passive not implemented)_
    - Claymore
      - Talking Stick
      - Tidal Shadow
    - Polearm
      - Ballad of the Fjords
      - Rightful Reward
    - Sword
      - Finale of the Deep
      - Fleuve Cendre Ferryman
      - Wolf-Fang

# 3.8.0

Note that this is non-comprehensive - up until creating this separate repo for issue tracking, we've just been listing important feature updates in the help page of the app.

Going forward we'll try to keep this up to date!

## Editor

- Interactive drag/drop editor for team rotation diagrams
- Keyboard entry support
- Animated timer
- Add all current characters' data, avatars, and action icons
- Add support for all traveler elements
- Undo/redo support
- Cooldown reset support
- Multicast action support
- Native support for talents which switch state (e.g. Cyno's burst, Ayato's skill, etc)
- Support for both self-infusion and general infusions
- Support constellations which alter cooldowns, buff durations, talent resets, infusions, and multicast counts
- Hitlag extension support (unclear how accurate the data is though - if you spot any discrepancies please create an issue)
- Support for cancellable actions (Yelan's and Sayu's skills)
- Implemented Childe kinda sorta maybe? Would appreciate it if a Childe user could confirm!
- Equippable weapons (including Sacrificial series skill cooldown reset)
- Animation cancelling via Dash button
- Customisable duration for claymore charged attacks
- Equippable artifacts

## Settings

- Multiple optimisation options for action timings
- Slider to simulate latency between actions and when switching characters
- Option to visually display animation durations, time markers, and animated timer
- Allow users to enter constellations

## Import/Export

- Save multiple teams locally
- Ability to import/export rotations via both link and text notation
- Ability to export rotations in code intended for gcsim
- Ability export rotations as an image, with basic background colour & transparency options
- Prebuilt team examples
