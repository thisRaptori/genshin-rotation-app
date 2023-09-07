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
