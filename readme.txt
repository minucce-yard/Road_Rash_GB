Road Rash (USA, Europe).gb


MD-5:  71AF355CBF7B8C7FE30F509803BBCED6
SHA-1: 488E699490598234E762ECF864C75EDCB1BC6066



______________________________________________________________



Minimum: critical fixes


gbc_compatible.ips
*  Playable on Color, Advance handhelds




road_width_compute.ips
*  Fix math algorithm for far distant road stretches
-  Prevent rare game lockups



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<



Basic: priority fixes


distant_car_visible.ips
*  Keep distant vehicles visible




hud_sprite_top.ips
*  Draw world sprites behind dashboard
*  Reduce road pixel flicker




menu_border_top.ips
*  Use correct tilemap at top of menu screen




portrait_frame_corner.ips
*  Fill in missing corner pixels on briefing portraits




prepare_road_tables.ips
*  Reduce mid-road tearing during drawing




sky_border_top.ips
*  Show cloud tiles on first lines of screen, instead of black corruption
-  Includes gbc_compatible patch




sky_clouds_align.ips
*  Correctly draw each sky texture line




stage_loading_delay.ips
*  Prevent slowdowns that greatly increase loading times




zero_money_printer.ips
*  Print $0 when broke or free item



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<



Plus: recommended fixes


better_transfer_speed.ips
*  Manage video timing to avoid longer loading times




player_rival_distance.ips
*  Compute correct distance values from other drivers




racer_name_symbols.ips
*  Add ' symbol to police names




script_text_format.ips
*  Re-centers dialogue for easier reading




speed_meter_precision.ips
*  Use more digits in printing speedometer




taller_bold_4.ips
*  Redrawn bold #4 digit to be more readable



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<



Special: minor fixes, enhancements


course_briefing_reorder.ips
*  Stage 1:
   -  Show regular dialogue on first play
   -  Show alternate text on course replay


*  Add Sergio's unused lines on race replays
   -  Level 4 = Pacific Coast
   -  Level 4 = Grass Valley
   -  Level 5 = Sierra Nevada


#  Requires rom_battery_expansion




double_speed_hack.ips
*  Turn on double speed DMG mode

#  Emulator hack required




final_standing_rivals.ips
*  Lock each driver's rank after crossing the finish line

#  Performance penalty




forfeit_race_early 
*  Drop out of race before it starts with no penalty  (pause game, then A + B + SELECT + START)
   Easier access to bike shop by skipping race

#  Requires rom_battery_expansion




password_battery_save
*  Auto-save progress after every race. Also saves player name.

   To reload save game, goto password screen
   - B + START = last password
   - A + START = last finished race
   - B + A + START = stage complete

#  Requires rom_battery_expansion




player_rank_precision.ips
*  Use more digits to determine accurate driver ranking
-  Includes player_rival_distance

#  Performance penalty




racer_sort_priority.ips
*  Print closest rivals who have higher veteran status

#  Performance penalty




rom_battery_expansion.ips
*  Expands MMC1 ROM to 256 KB
   Adds battery 2KB SRAM




skip_splash_screen.ips
*  Press joypad button to skip logo screen




sky_animate_last.ips
*  Move last line of clouds at skyline  (very very slow)

#  Performance penalty



_______________________________________________



Commits:


26.3 - [2021-08-29]
*  cleanup



26.2 - [2021-08-29]
*  re-sort patches, based on performance



26.1 - [2021-08-28]
*  better_transfer_speed updated
   -  fix oam refresh menu timing glitch



26 - [2021-08-27]
*  password_battery_save released



25.2 - [2021-08-26]
*  forfeit_race_early updated
   -  keep on rank on level replays
   -  reset timers to prevent odd glitches



25.1 - [2021-08-24]
*  player_rival_distance updated
   -  simplify patch  [player_rank_precision]



25 - [2021-08-23]
*  road_width_compute released



24 - [2021-08-21]
*  forfeit_race_early released



23 - [2021-08-20]
*  script_text_format released



22.1 - [2021-08-18]
*  menu_border_top updated
   better_transfer_speed updated
   -  IRQ exit during h-blank to fix rare timing glitches



22 - [2021-08-17]
*  course_briefing_reorder released
   rom_battery_expansion released



21.2 - [2021-08-16]
*  cleanup



21.1 - [2021-08-15]
*  better_transfer_speed updated
   -  little faster overall



21 - [2021-08-14]
*  prepare_road_tables released



20 - [2021-08-14]
*  distant_car_visible released



19.3 - [2021-08-13]
*  sky_border_top updated
   -  reduce sky flicker  [original]



19.2 - [2021-08-12]
*  hud_sprite_top updated
   -  reduce road flicker  [original]



19.1 - [2021-08-11]
*  sky_clouds_align updated
   -  rare flicker glitch  [original]



19 - [2021-08-09]
*  final_standing_rivals released



18 - [2021-08-07]
*  player_rank_precision released



17 - [2021-08-05]
*  player_rival_distance released



16 - [2021-08-03]
*  speed_meter_precision released



15 - [2021-08-01]
*  racer_sort_priority released



14 - [2021-07-30]
*  racer_name_letters released



13 - [2021-07-28]
*  double_speed_hack released



12.1 - [2021-07-26]
*  re-organize



12 - [2021-07-25]
*  skip_splash_screen released



11.2 - [2021-07-25]
*  adc fixes
   -  sky_border_top
   -  write_world_map
   -  write_world_sprite



11a - [2021-07-24]
*  cleanup - rename files



11 - [2021-07-24]
*  sky_animate_last released



10a - [2021-07-23]
*  cleanup - rename files



10 - [2021-07-23]
*  taller_bold_4 released



9 - [2021-07-22]
*  portrait_frame_corner released



8 - [2021-07-21]
*  zero_money_printer released



7 - [2021-07-19]
*  better_loading_speed released



6 - [2021-07-17]
*  sky_clouds_align released



5 - [2021-07-15]
*  sky_border_top released



4 - [2021-07-13]
*  stage_loading_delay released



3__2021-07-11
*  menu_border_top released



2__2021-07-09
*  hud_sprite_top released



1__2021-07-07
*  gbc_compatible released



_______________________________________________



Visit:
*  https://github.com/minucce-yard/Road_Rash_GB




Helpful:
*  BGB -- incredibly helpful debugger
*  SameBoy -- very high recreation of Game Boy



_______________________________________________



Comments:


*  PRESS select button
   -  Course select: opens password, name menu
   -  Password: opens credits screen
   -  In-game race: shows bike health
   -  Post-race results: opens bike shop menu



*  In-game soft reset: keep holding A + B + Select + Start



*  Sometimes you'll see the same racer names repeatedly
   -  When some rivals fall behind, they can aggressively cling to your tail

   -  Some rashers have different bikes, with major (de-)acceleration bonuses
      If you're fast, you can see them zip up the ranks in the distance

   -  During player crashes, veterans who are far ahead will actually take a break
      When the player resumes driving, they will re-start their bikes



*  Stage clear: place 4th or higher in each course
   -  Passwords are reset after the promotion screen
      Check options menu for new code afterward



*  Higher stages require better bikes
   -  Replaying finished courses is a faster way to save up money



*  Shopping cart:
   -  Empty



*  For best performance, use an emulator that supports double-speed DMG mode  (overclock hack)



*  Hardware limitations:
   -  When lots of sprites on-screen (2 cars + several racers), tiles may briefly drop out.



*  Scrapbook of unbuilt expansion modules


   30 fps
   -  Seems unrealistic on DMG. Sprite engine could run better.
      Probably some waste of cycles scattered everywhere. Lots of work.


   Colorizer
   -  There's not much color to add: menus, portraits, sprites, title, clouds, mountains, road.
      Still feels like enough work.


   Expanded font
   -  Add lower-case letters  (4x8 thin, 8x8 bold)



*  Alternate version: beta or early release
   -  Camera angle is at ground level, making far objects hard to spot
   -  Runs faster with few graphical glitches, due to more rendering time
   -  Rivals seem to fight less



*  RAM cheats:

   d11b = 1-5  [level #]


   d11c = 0-5  [sierra nevada]
   d11d = 0-5  [pacific coast]
   d11e = 0-5  [redwood forest]
   d11f = 0-5  [palm forest]
   d120 = 0-5  [grass valley]

   d121 = 0-5  [bike]

   d122-d123 = money  [16-bit lsb]
   -  0012 = $1200
   -  1000 = $100000



   d01c-d01d = race distance  [16-bit lsb]
   -  07e0 ~ 5.6 miles


   d01e-d020 = distance driven  [24-bit lsb]
   -  07e000 ~ 5.6 miles


   cfe5 = speed  [16-bit lsb]
   -  $94 * (3/4) ==> $6f  [111 mph]


   ce63 = race transition timer
   -  $00 = racing
   -  $02 = end race


   ce65 = race flag
   -  $00 = normal
   -  $01 = busted


   ce66 = race flag
   -  $00 = normal
   -  $01 = wrecked


   ce0a = police flag
   -  $00 = on-duty
   -  $01 = off-duty



_________________________________________________________



Compile:

*  Z80 armips assembler by Prof9
   https://github.com/Prof9/armips/tree/gameboy



*  Copy @__build files to root folder  (one up)

   armips "road_rash.asm.txt"
   rgbfix -fgh "Road Rash (USA, Europe).gb"
