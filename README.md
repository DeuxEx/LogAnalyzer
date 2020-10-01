# LogAnalyzer
LogAnalyzer (for Entropia Universe logfile) (MMO RCE)

Version 1.0.0.26
--------------------------------------

GUI driven skills analyzer and screenshot of active window when globaling.

Put both files (.exe and .ini) in C:\LogAnalyzer folder (if you dont have one you must create it)

In this folder subfolders (with current date/time) are created when everything is filled out and you press start.

In the subfolder directories files are exported and screenshots are created.

Exported file (LogAnalyzer_globals.txt) contains all globals.

Exported file (skillsoutfile.txt) contains all skills gotten during the session.

--------------------------------------


The filtered logview:

Alot of keywords are removed from this field in the GUI, so the most importants are kept and showed here.

--------------------------------------

The skills field:

All skills which are increasing are captured and displayed in a sorted list in one field of the GUI.

Every 20th skill increase this sorted list is exported to an file called skillsoutfile.txt.

--------------------------------------

Screenshots:

Are taken when avatar and team name are globalling.

Names on the files include the item/mob and the value.

The screenshot is taken with a 1200 millisec delay, i found this value to be working allright. (Can be an variable in the future)

--------------------------------------

The inifile:

An inifile are read during the execution start of GUI and there are currently 4 values read from this file:

The active lines starts with [1],[2],[3] of [4], watch how I have typed in the examplefile.

[1]Avatarname

[2]Teamname

[3]Followmode

[4]Logfile path and filename

--------------------------------------

Followmode:

When Followmode are given in the inifile or written in the GUI, the loganalyzer is displaying all the full lines containing this keyword in one field of the GUI.

Followmode can ie be; [Society] 

If you want to have all society activity in the field.

Or any kind of mobs or crafting or mining texts.

This feature is somewhere buggy and if you want to change the string, close down the GUI and restart it before running.

--------------------------------------

Importance field:

In this field rare items are displayed, tier increasing items and ATHs.

--------------------------------------

Bugs:

*Sometimes the code crashed and that can happen if you stopped and restarted via the buttons.

Best way to solve this is to stop the cmd/powershell process from where you started the Loganalyzer, and have a fresh restart on it.

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

Send thx or bug-reports to; deux.ex@gpromm.com

--------------------------------------

Love from

Deux Pelleman Ex
