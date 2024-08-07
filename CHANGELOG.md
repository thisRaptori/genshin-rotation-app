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
