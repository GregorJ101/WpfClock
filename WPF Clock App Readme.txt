WPF Clock App

This app is written entirely in C# using WPF.  It began with a very simple
C#/WPF clock app downloadeded from the Web
(http://www.c-sharpcorner.com/blogs/digital-clock-in-wpf1)
and has been enhanced and extended significantly:
- Hid title bar
- Added code to drag window without a title bar
- Updates calendar each time the app gets activated (to keep date current
    after the OS is awakened from sleep or hibernation)
- Added context menu
- Added multiple date formats
- Added code to toggle topmost & draggable states
- Added checkboxes to each stateful context menu item
- Applied radio-control model mutual exclusion to date format settings and
    display mode settings
- Added code to save window position to registry on exit and restore to
    last position on startup
- Added no-date menu option
- Added 24-hour menu option
- Ctrl-T to toggle always-on-top state
- Added copying date & time to clipboard
- Added transparent window background option
- Added variable window background opacity
- Added "Close and remove settings" menu option to remove all registry
    entries
- Added code to adjust border thickness dynamically
- Mapped + & - keys to increase & decrease border thickness
- Added "/t" command-line argument to show title bar
- Added code to switch between 3 title bar border formats
- Added simple About box
- Added code to close About box on Escape keystroke
- Added Windows Vista/7 "glass" background
- Added code to limit border thickness to 9 and deactivate "increase border
    thickness" menu item conditionally

Many more changes have been made since this initial list.  See the file "Wpf Clock App.pdf" and "Wpf Clock Change.log" for more detail.

Installation is very simple: just copy it wherever it is desired and run it.
The settings are saved in the registry and are loaded each time the app is started.

All the settings are available only in the context menu.  Right-click anywhere in
the app's window to get it to pop up.

CAUTION: When the "Click-through" menu option is selected, all mouse events will
pass through any part of the window where the background is visible.  To create
the context menu, first locate the sharp tip of the mouse cursor on some part of
the display that has text, then right-click to create the menu.  If no context
menu shows or the context menu of the window behind the clock is shown, just try
again until the clock app menu shows.  The "click-through" option is disabled by
default.

A "usage" message box is available by using the "/?" command line option.

To remove the app, first select the "Close and remove settings" menu option which
will remove all the keys and values saved in the system registry, then just delete
the .exe file.  Done.

Comments may be sent to greg02@pobox.com.
