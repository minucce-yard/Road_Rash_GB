Road Rash (USA, Europe).gb



______________________________________________________________



Basic:


gbc_compatible.ips
*  Playable on Color, Advance handhelds



hud_sprite_top.ips
*  Draw world sprites behind dashboard



menu_border_top.ips
*  Use correct tilemap at top of menu screen



portrait_frame_corner.ips
*  Fill in missing corner pixels on briefing portraits



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



Plus:


better_loading_speed.ips
*  Manage video timing to avoid longer loading times



racer_name_letters.ips
*  Add ' symbol to police names



racer_sort_priority.ips
*  Print closest rivals who have higher veteran status



skip_splash_screen.ips
*  Press joypad button to skip logo screen



sky_animate_last.ips
*  Move last line of clouds at skyline



taller_bold_4.ips
*  Redrawn bold #4 digit to be more readable



<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<



Special:


double_speed_hack.ips
*  Turn on double speed DMG mode
-  Emulator hack required



_______________________________________________



Commits:


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
   -  Race course: opens password, name menu
   -  Password: opens credits screen
   -  In-game race: shows bike health
   -  Race results: opens bike shop menu



*  In-game soft reset: press A + B + Select + Start



*  Sometimes you'll see the same racer names repeatedly.
   -  When some rivals fall behind, they can aggressively cling to your tail.

   -  Some rashers have different bikes, with major (de-)acceleration bonuses.
      If you're fast, you can see them zip up the ranks in the distance.

   -  During player crashes, veterans who are far ahead will actually take a break.
      When the player resumes driving, they will re-start their bikes.



*  Shopping cart:
   -  Sometimes sky flickers due to bad mis-timing when creating scroll info
   -  Menu loading times can be somewhat improved perhaps
   -  Re-center dialogue text for less awkward spaces
   -  Sergio has 3 unused lines. Find way to add extra text?



*  For best performance, use an emulator that supports double-speed DMG mode  (overclock hack)



*  Hardware limitations:

   - When lots of sprites on-screen (2 cars + several racers), tiles may briefly drop out.
     Road may also flicker during these events.



*  RAM cheats:

   d11b = 1-5  [level #]


   d11c = 0-5  [sierra nevada]
   d11d = 0-5  [pacific coast]
   d11e = 0-5  [redwood forest]
   d11f = 0-5  [palm forest]
   d120 = 0-5  [grass valley]


   d122-d123 = money  [16-bit lsb]
   -  0012 = $1200
   -  1000 = $100000


   d01e-d020 = distance driven  [24-bit lsb]
   -  07dfe3 ~ 5.6 miles



_________________________________________________________



Compile:

*  Z80 armips assembler by Prof9
   https://github.com/Prof9/armips/tree/gameboy



*  Copy @__build files to root folder  (one up)

   armips "road_rash.asm.txt"
   rgbfix -fgh "Road Rash (USA, Europe).gb"
