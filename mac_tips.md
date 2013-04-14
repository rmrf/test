Piping Output into Default GUI Apps

    ls -la | open -f
    ls -la | open -f -a TextMate
    ls -la | pbcopy

Paste Clipboard conetent into a file(usefull for extra large copy, even very slow for vi)

    pbpaste > clipboard_content.txt

Know exactly where you are in Finder:

    $ defaults write com.apple.finder PathBarRootAtHome -bool TRUE;killall Finder

Show Full Paths in the Title Bar of Finder:

    $ defaults write com.apple.finder _FXShowPosixPathInTitle -bool TRUE; killall Finder

Hidden Files and folders:

    chflags hidden secret.doc

Unhindden:

    chflags nohidden secret.doc


Shutdown, reboot box:

    Control + Eject


Reset Your Mac’s Hardware Settings

    To do so on a portable Mac that has a battery that can’t be removed, shut down the computer and ensure the power cable is attached. Then hold down Shift + Control + Option and press the power button. Release, then restart your computer in the usual way.

Resetting the Parameter RAM (PRAM) 

    reboot and—before the Apple logo appears and you hear the boot-time chime—hold down 
    Command and Option , then hold P and R . 
    The system will restart. Release all keys and let the computer boot as usual.


View Tech Info at the Mac Login Screen:

    sudo defaults write /Library/Preferences/com.apple.loginwindow AdminHostInfo 1

Rever it 

    sudo defaults delete /Library/Preferences/com.apple.loginwindow AdminHostInfo



Screenshot

    Shift + Command +3 , for whole desktop
    Shift + Command + 4 , select the space need snapshot
    Shift + Command + 4 , then tap Space . Then click the window you want to capture.


Select Text as pro

    1, in some app, such as TextEdit or Firefox, click and select text , then hold CMD then select other text, you will got multi select 

    2, option key,rectangular blocks of text within a paragraph.   


Change the Login Screen Wallpaper

    The file we need to replace is called NSTexturedFullScreenBackgroundColor.png and is located at /System/Library/Frameworks/AppKit.framework/Versions/C/Resources/. 


Download the update:

    1, list it
    sudo softwareupdate -l

    2, download and install:
    sudo softwareupdate -i MacOSXUpd10.7.1-10.7.1

    3, only download 
    sudo softwareupdate -d MacOSXUpd10.7.1-10.7.1

    4, To download but not install all available updates,

    sudo softwareupdate -d -a


Deactivating the Writing of .DS_store Files on Networks

    defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool TRUE

Reverting to Default

    defaults delete com.apple.desktopservices DSDontWriteNetworkStores


Boot Related:

    By holding down various key combinations before the Apple logo first appears when booting, 

    CMD - R : boot to recovery mode
    CMD - S : Sigle user mode

    Option: Switch between operating systems installed on your comput- er 
    Shift: Boot into safe mode,
    C: boot from CD/DVD
    N: Network boot
    X: Force Mac OS X to boot.

    CMD - V: Boot in verbose mode, showing boot time messages rather than the Apple logo. 

    Eject button: Eject any inserted CD/DVD (holding the mouse button does the same thing).


Open a file with spetial app

    open -a Mail Disneyland.jpg


Activating the Root Account

    /System/Library/CoreServices.
    open Directory Utility program.
