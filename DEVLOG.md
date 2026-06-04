LOG BOOK

26.05.2026 PROGRESS (DAY 1):

- Created the initial survival game concept and flow
- Added core game data dictionaries:
  - ANIMALS
  - EXPERTISES
  - LOCATIONS
- Defined animal stats like: meat amount, risk, encounter chance and damage.
- Added location data with available animals and descriptions.
- Rebuilt user_choice() from memory after using it in previous text-based-RPG project for reusable input validation.
- Added location selection and travel logic with location_choice() and travel().
- Created the first version of the player set-up with name, expertise, health, and food.
- Built the hunting system using random animal encounters, risk rolls, health loss, and food gain.
- Created following functions: user_choice(prompt, valid_choices), location_choice(), travel(), hunt(player, location), show_status(player, current_location), take_action(), rest(player)

27.05.2026 PROGRESS (DAY 2):
- Cleaner overall code structure and improved readability
- Added create_player(name, expertise) for better player set-up
- Added main() for better game start-up and loop
- Added expertises and working bonuses:
   - Navigator improves encounter chance
   - Hunter lowers hunt failure and injury risk
   - Cook improves food gain scaling
- Rebuilt hunt function from memory
- Fixed multiple syntax, logic and state-management bugs + issues

28.05.2026 PROGRESS (DAY 3):
- Added option to disengage from animal encounter into the hunt function
- Added 3 new animals (wolf, bison, moose)
- Added Inventory system and proper display
- Added new loot variant (misc)
- Split show_status function into show_inventory and show_status
- show_status no longer shows without player's input during take_action menu
- Added hunger, depletes by 10-20 depending on action
- Significantly reduced AI reliance
- Added eat(player) function
- Increased encounter chances
- Fixed capitalization

29.05.2026 PROGRESS (DAY 4):
- Added day counter
- Added energy system
- Added energy_req(player, amount)
- Added hunger_loss(player, amount)
- Updated hunt and travel to require energy
- Rest now restores health and energy
- Improved eat(player) 

30.05.2026 PROGRESS (DAY 5):
- Added Camping System
- Added Camp-Exclusive Actions
- Added Fishing and Fish Variables Group
- Added choose_fish function with upgraded RNG system
- Rebalanced energy and food variables
- Split action choices into several lines instead of single lines for increased readability and comfort
- Quick debugging of common issues through pattern recognition

31.05.2026 PROGRESS (DAY 6):
- Fishes are no longer guaranteed to appear
- Added Materials into the Dictionary
- Added gather_wood and choose_wood_event functions
- Added wood_events dictionary
- Add gather_wood as a camp action

01.06.2026 PROGRESS (DAY 7):
- Reconstructed choose_wood_event() and choose_fish()
- Fixed bugs in gather_wood(player) and choose_wood_event()
- Added Building variables
- Added build_action()
- Added build(), unfinished
- Laid foundations for building mechanics

02.06.2026 PROGRESS (DAY 8):
- Finished build(player)
- Added build(player) to the camp()
- Added working bonuses for buildings
- Added "buildings" section to create_player(name, expertise)
- Expanded rest(player) to include max_energy calculated based off buildings inside create_player(name, expertise)
- Expanded eat(player) to include max_hunger calculated based off buildings inside create_player(name, expertise)
- Updated outdated variable names
- Fixed logical flaws in hunt(), fish(), rest(), build_action()
- Updated show_inventory() and show_status()
- Added materials section in the create_player(), housing crafting materials
- Updated recipes for buildings and MATERIALS dictionary
- Updated every ['inventory']['wood'] to ['inventory']['materials']['wood']

03.06.2026 PROGRESS (DAY 9): 
- Added crafting() and implemented into the camp()
- Finished crafting system
- Fixed Materials list in create_player()
- Fixed indentation for "misc" in create_player() and moved it inside "inventory"
- Added dynamic health output in UI for rest()

04.06.2026 ENDING (DAY 10):
- Added building upgrades
- Added get_max_hunger()
- Added win condition
- Project concluded
