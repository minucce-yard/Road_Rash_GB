Road Rash (USA, Europe).gb



______________________________________________________________



Fixes:


better_loading_speed.ips
*  Manage video timing to avoid longer loading times



gbc_compatible.ips
*  Playable on Color, Advance handhelds



hud_sprite_top.ips
*  Draw world sprites behind dashboard



menu_border_top.ips
*  Use correct tilemap at top of menu screen



portrait_frame_corner.ips
*  Fill in missing corner pixels on briefing portraits



sky_animate_last.ips
*  Move last line of clouds at skyline



sky_border_top.ips
*  Show cloud tiles on first lines of screen, instead of black corruption

-  Includes gbc_compatible patch



sky_clouds_align.ips
*  Correctly draw each sky texture line



stage_loading_delay.ips
*  Prevent slowdowns that greatly increase loading times



taller_bold_4.ips
*  Redrawn bold #4 digit to be more readable



zero_money_printer.ips
*  Print $0 when broke or free item



_______________________________________________



Commits:


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



*  Shopping cart:
   -  Add (') marks to in-game police names
   -  Sometimes sky flickers due to bad mis-timing when creating scroll info.
   -  Create way to skip logo splash screen
   -  Races run at 22-25 instead of 30 fps. Improve frame speed?
   -  Menu loading times can be somewhat improved perhaps
   -  Re-center dialogue text for less awkward spaces
   -  Activate double speed mode (GBC emulator only?)
   -  Remove world object sprite flicker  (GBC emulator with no sprite limit?)
   -  Look at sound engine for any mistakes, since Code Monkeys engine has lots of minor flaws
   -  Sergio has 3 unused lines. Find way to add extra text?
   -  Check hud racer name
   -  Inspect unusual car sprites disappearing briefly



*  RAM cheats:

   d11b = 1-5  [level #]


   d11c = 0-5  [sierra nevada]
   d11d = 0-5  [pacific coast]
   d11e = 0-5  [redwood forest]
   d11f = 0-5  [palm forest]
   d120 = 0-5  [grass valley]


   d122 = money  [16-bit]
   -  0012 = $1200
   -  1000 = $100000
