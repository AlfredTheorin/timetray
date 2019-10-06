# TimeTray
TimeTray displays the current calender week in a system tray

## Install/Usage
If you don't use the "Download ZIP" option but only want to download _TimeTray.jar_, **don't right-click it in the list (!) but left-click on it and get the "RAW" version**!

Just make sure that you're running a Java Runtime Environment (e. g. the [JRE from Oracle](http://www.java.com/en/download/ "Oracle")), and put _TimeTray.bat_ into your autostart folder, crontab, whatever...

## Screenshot
![timetray](https://github.com/otacke/timetray/blob/master/timetray.png "timetray")

## Additional Information
TimeTray is a very simple program that I originally hacked on one day for a former colleague of mine many years ago. It displays the current calender week in a system tray -- a feature that Windows still lacks in 2016. Since TimeTray is written in Java, it can run on other operating systems as well, e.g. Linux or MacOS.

TimeTray is totally working -- I hope ;-) Anyway, allowing to set (and save) some parameters would be useful:

* the tray icon's background color
* the tray icon's font color
* the tray icon's font
* time zone and locale 

So far, there is a rudimental settings window that just tells you where to edit the settings in a plain text file called _.timetray_ in your home directory. You can edit the file with a text editor line by line to change other values. The lines mean...

1. (0-255) red value of the TrayIcon's background color
2. (0-255) green value of the TrayIcon's background color
3. (0-255) blue value of the TrayIcon's background color
4. (0-255) alpha value of the TrayIcon's background color
5. (0-255) red value of the font color
6. (0-255) green value of the font color
7. (0-255) blue value of the font color
8. (0-255) alpha value of the font color
9. name of the font family
10. number representing the font style (I didn't look up which number means what, but 0 is plain)
11. simple date format pattern representing the format for the TrayIcons toolstip text
12. time zone
13. locale language
14. locale country

The load and save routines are only rudimentary, so you might crash TimeTray if you set illegal values. In doubt, delete .timetray in your home directory. TimeTray will then reset the file if neccessary. The ugly routines should probably be improved...

_When will all this be done? When it's done. But to be honest: I don't care much about this piece of code that's probably mainly used for Windows. Sorry! But you may use the source, Luke!_

## License
TimeTray is licensed under the [DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE](http://www.wtfpl.net).
