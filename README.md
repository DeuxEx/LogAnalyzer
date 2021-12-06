# LogAnalyzer
LogAnalyzer (for Entropia Universe logfile) (MMO RCE)

Version 1.0.0.78

Download it here:
https://github.com/DeuxEx/LogAnalyzer/releases/tag/v1.0.0.78

Project development info:
https://github.com/DeuxEx/LogAnalyzer/projects/1

--------------------------------------

GUI driven skills analyzer and screenshot of active window when globaling.

Ths msi installer creates c:\Loganalyzer and puts the inifile and the gifs in there.

In this folder, subfolders (with current date/time) are created when everything is filled out and you press start.

In the subfolder directories files are exported and screenshots are created.


--------------------------------------


The filtered logview:

Alot of keywords are removed from this field in the GUI, so the most importants are kept and showed here.

--------------------------------------

The skills field:

All skills which are increasing are captured and displayed in a sorted list in one field of the GUI.


--------------------------------------

Screenshots:

Are taken when avatar and/or team name are globalling.

Names on the files include the item/mob and the value.

The screenshot is taken with a 1200 millisec delay, i found this value to be working allright. (Can be an variable in the future)

--------------------------------------

The inifile:

An inifile are read when you click the "Read inifile" button, and there are currently 4 values read from this file:

The active lines starts with [1],[2],[3] of [4], watch how I have typed in the examplefile.

[1]Avatarname

[2]Teamname

[3]Followmode

[4]Logfile path and filename

--------------------------------------

Followmode:

When Followmode are given in the inifile or written in the GUI, the loganalyzer is displaying all the full lines containing this keyword in one field of the GUI.

Followmode can ie be; [Society] 

If you want to have all society activity in the field, or any kind of mobs or crafting or mining texts.

--------------------------------------

Importance field:

In this field rare items are displayed, tier increasing items and ATHs.

--------------------------------------


When you or the team global, a file is renamed in the LogAnalyzer folder, this file can be linked to while streaming so it will show an animated gif.
Also if you are using following function in LogAnalyzer, and if the followstring is met another file is renamed in the LogAnalyzer folder.
These two files are hardcoded atm, and the names are:
sherlock_gnomes_spins.gif for the global
follow_star.gif for the follow.

In streamlabs you configure these files and place them on the screen and when you are ready, you rename the links in streamlabs to point to these files but add ".inactive" in the end of the filenames so they dont show up.
When a global or a follow later is being hit in LogAnalyzer these files (if found) are renamed for 10 seconds and then renamed back again.


--------------------------------------



Details:

All code is done in C# (Visual Studio 2019)

Framework used is .NET 4.7.2

--------------------------------------

Others:

The GUI code is working great at my place, with some bugs, but still works great.

The counting of skills in the field is the code I put most effort in, and the collecting, adding and sorting routines are really fast.

Dont ask about future improvements or features.

The code is changed and improved on a regular basis.

Send thx, bug-reports or paypal money to; deux.ex@gpromm.com

--------------------------------------

Love from

Deux Pelleman Ex
