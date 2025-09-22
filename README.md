# poe2
simple batch file to fix cpu affinities 		
* the bat file is based on my cores which is 20, you should edit the mask for yours. and (11111111111111111100 converted to hex is ffffc) remove or add cores then decimal to hex converter, or use https://bitsum.com/tools/cpu-affinity-calculator/ and copy only the part with values other than 0. 
* %comspec% /C start /normal /affinity ffffc PathOfExileSteam.exe  
   is the bat file line, (based on steam version, change if your exe is different)
*	place the file in your poe2 folder, if steam right click on the game, manage, local files. you save it here then on the top copy the directory address. E:\SteamLibrary\steamapps\common\Path of Exile 2 is mine for instance
*	if you use steam right click on the game in general launch options paste this without the half circles (  "address you copied" %command%    ) needs the quotation marks and percent signs command.
*	if it's not you edit the the shortcut you use to launch it the target field write (   C:\Windows\System32\cmd.exe /C start "" /affinity ffffc "path to program shoudl be under it so paste here" (add \ProgramName.exe at the end before the last quotation mark
*  if everything was done correctly likely windows will ask if you trust it, and also if you want to confirm each time you open. i'd turn off the confirm personally 
