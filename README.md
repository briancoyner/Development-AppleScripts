# AppleScripts
## Created by Brian Coyner, 2011

## Resize Xcode
### Description
This AppleScript (also available as an executable application bundle) re-sizes and re-positions all open Xcode windows. The committed script contains a size and position suitable for a Apple 27" Cinema display. The size and position is perfect for how I want Xcode to look. You can change the script to size and position the Xcode windows anyway you like.

### How to use
Use Spotlight to quickly execute the AppleScript app bundle. Simply type Command+Space, Resize Xcode, Return. Once you execute the script a couple of times, Spotlight is really fast at displaying the script in the popover menu.

### Why use it?
If you find yourself moving Xcode windows around a lot, then you will love this script because it allows you to quickly size and position your Xcode windows just the way you like. For example, I often move around Xcode windows when comparing source from multiple projects. Once I am done, my Xcode windows are all over the screen. A quick Command+Space, Resize Xcode, Return, and my Xcode windows are perfectly sized and positioned.

### I don't like your size and position. How do I change it?
Open the the 'Resize Xcode.app' application bundle or the 'Resize Xcode.scpt' file using AppleScript Editor. Then modify the size and/ or position values. 

### What does the script look like?

    tell application "Xcode"
        -- using 9999 as the height automatically takes into account the size of the dock
        set the bounds of every window to {400, 0, 400 + 1900, 9999}
    end tell
