# AlwaysOnTop

This allows you to lock windows always visible on top of the screen.

HOW TO USE

- Run the program
- Select the windows you want lock and press "ALT + SPACE"

When you run the program, the process remains running in the background, you can see the icon appear at the bottom right, where you can also stop it.

You can lock windows at any time, even multiple windows at the same time, by simply clicking on the window you want to lock and pressing the key combination "ALT + SPACE"
Select a locked windows and press the combination again to remove the lock.

SCRIPT

I used AutoHotKey to create the program and convert it to .exe

This is the script i used:
I_Icon = aotIcon.ico
IfExist, %I_Icon%
  Menu, Tray, Icon, %I_Icon%

!SPACE::  Winset, Alwaysontop, , A
