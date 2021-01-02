# Elder Scrolls Online Addons Collection
A collection of popular addons created by me for the game, Elder Scrolls Online

Website: https://www.esoui.com/downloads/author-52033.html

* [Crystal Fragments Proc](#crystal-fragments-proc)
* [Ward Shield Reminder](#ward-shield-reminder)
* [Installation](#installation)
* [Special Thanks](#special-thanks)  

## Crystal Fragments Proc

Website: https://www.esoui.com/downloads/info2441-CrystalFragmentsProc.html#info

**Current Version**: v1.5

**This addon detects when the ability, Crystal Fragments, triggers the effect of granting the next use of 'Crystal Fragments' (Sorcerer's skill) as an instant cast ability with 50% cost of magicka and 20% more damage. It then alerts the user by displaying a big icon, along with a timer, on the screen. Position of the icon can be adjusted and its new location will be automatically saved for future play sessions. The icon disappears as soon as it is casted or if buff duration is over.**

*Inspired by Reager's now-discontinued addon of the same name*: https://www.esoui.com/downloads/info443-CrystalFragmentsProc.html

To adjust the position of the icon:
- /cfp show - Displays location of the icon. Simply use your mouse to drag it to your desired position.
- /cfp hide - Hides the indicator after icon is at your desired position.

To adjust the size of the icon and timer text (Requires LibAddOnMenu!):
Access Crystal Fragments Proc's addon settings -
Press Esc -> Settings -> Addon -> Crystal Fragments Proc -> Adjust accordingly.

To save computing resources, the add-on will only activate for Sorcerers.

### Change Log:

v1.5 (July 29, 2020):
- The addon should now work with any version of this game.
- Default timer size is now bigger.
- The indicator (image and text) are now adjustable to a certain point. (Requires LibAddOnMenu!)
- Maintenance (documentation)

v1.4 (March 1, 2020):
- Fixed a bug where the addon might conflict with another. (Thanks, Nyyxxon!)
- Maintenance (matching APIVersion, documentation)

v1.3 (August 18, 2019):
- Timer is now implemented in this addon. With this new feature, any bug that causes the alert icon to stay on the screen even when duration is over should now be fixed.
- Maintenance (matching APIVersion, documentation)

v1.2 (August 17, 2019):
- Fixed a bug where the addon was also detecting other player's Crystal Fragment procs. Had no effect on user, but this bug fix should help with performance.

v1.1 (August 16, 2019):
- Optimization
- Icon can now be moved. New location will be saved for future play sessions.
- Icon will remain visible until skill is casted or if duration is over

## Ward Shield Reminder

Website: https://www.esoui.com/downloads/info2456-WardShieldReminder.html

**Current version**: v1.1

**This addon detects when an activated damage shield is lower than an adjustable percentage threshold (Default is at 0.45 of shield strength) or an adjustable base threshold (default is at 2500), or if the shield has been deactivated or destroyed.** 

**It alerts the user by displaying a (WARD LOW!) warning on the screen when the user's damage shield is lower than a percentage threshold or a base threshold, or a (WARD DOWN!) warning if the damage shield has been destroyed or deactivated.** 

**Position of the icon can be adjusted and its new location will be automatically saved for future play sessions. The percentage threshold and base threshold can also be adjusted and its value will be automatically saved. The icon disappears as soon as the player is out of combat or if it the user has applied a new ward shield.**

*Inspired and made possible by @ratparol101's addon*: https://www.esoui.com/downloads/info1676-WardHelper.html *and Garkin's addon*: https://www.esoui.com/downloads/info799-ShieldInfo.html

For default values, percentage threshold is the value of shield strength * 0.45, meaning at 45% of the shield strength, the WARD LOW! alert will pop out.

Base threshold is 2500, meaning when shield strength is at 2500, the WARD LOW! alert will pop out.

To adjust the position and of the icon and the percentage threshold:  
- /wrm show - Displays location of the warning icon. Simply use your mouse to drag it to your desired position.  
- /wrm hide - Hides the indicator after warning icon is at your desired position.  
- /wrm value - Shows current threshold percentage.  
- /wrm '0.05-0.99' - To adjust the threshold percentage, simply type in a value after /wrm. It has to be between 0.05 or 0.99. Any other number will prompt a debug message telling the player that an invalid value has been inputted. For example, if you want to set the threshold to 0.35, type in /wrm 0.35. Default is at 0.45. (Recommended Values: 0.35-0.65)

To adjust the base threshold:
- /wrmb value - Shows current base threshold.  
- /wrmb '500-10000' - To adjust the base threshold percentage, simply type in a value after /wrmb. It has to be between 500 or 10000. Any other number will prompt a debug message telling the player that an invalid value has been inputted. For example, if you want to set the threshold to 1000, type in /wrmb 1000. Default is at 2500. (Recommended Values: 1000-3500)

Limitations:
- Percentage Threshold is changed every time a shield is destroyed or deactivated. This isn't normally a problem, but it could become one if a small shield was the only shield remaining. I had different iteration of this addon that doesn't do this, but it introduced new problems (mostly logical). For this iteration, the current fail-safe fix is a base threshold that the user can adjust. It kind of defeats the purpose of the percentage feature, so I am not sure if this is the right idea of going about it. Let me know if you have an idea of how you think this threshold should work.

- Multiple Shields might bug out the addon. So far, I have only been able to test it when I have Annulment and Hardened Ward activated (the only shield actives for Sorc). I am not sure what might happen if multiple shields from other players are applied to the userr as it is difficult to do complete testing by myself. The addon should still work fine, but let me know if a bug occurs in your playtime and how it happened, so I can try to fix it.

### Change Log
v1.1 (September 6, 2019):
- Removed class restriction; the addon can now be used with any class

# Installation  
You can install addons by using one of the following ways:
1. Download the files and extract them to your ESO Addon folder. The typical default install path is:  
```C:\Users\< username >\Documents\Elder Scrolls Online\live\AddOns.```  
Create one if it doesn't already exist.
2. Or download Minion. Instruction is available on their website: https://minion.mmoui.com/ 

# Special Thanks
ESO UI Wiki and Forums
