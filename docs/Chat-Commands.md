---
layout: home
title: Chat Commands
---
# List Chat Commands

(document version 0.2; thanks to Medea Destiny for writing most of this)   

Below is the complete list of chat commands.  What's listed are the calls after the prefix.  See [Prefixes, Chat Commands and Other Non-Menu Functions](/docs/Prefixes,-Chat-Commands-and-Other-Non-Menu-Functions) for how to learn, use, and change the wearer's prefix.
Help us make this list complete ! Please submit any chat commands you find that are not listed here, or ones that are listed here that no longer work, via pull request to this page.

**IMPORTANT:** 
* Many chat commands do not *need* a space after the prefix but some do, especially chat commands with more than a single term.  All chat commands do work with a space after the prefix.  
* Not all chat commands are case-insensitive (i.e some will require you to capitalize things correctly). If you see a command in the list below with a capital letter, you have to use it in that form. When you're referring to a specific function (for example the name of an animation or a restriction preset), use the capitalization of that animation, function, etc. There are a few places where we've made things case-insensitive, but not everywhere. If something doesn't work as expected, check your capitalization.
  
## MENU SHORTCUTS

### Primary menus:

`menu` calls the Main Menu   
   
`access`  calls the Access (formerly "auth") Menu  
`animations` or `menu animations` calls the Animations Menu   
`apps`  calls the Apps Menu  
`exceptions` calls the Exceptions Menu in RLV  
`help/about`  calls the Help/about Menu    
`leashmenu` calls the Leash Menu   
`relay` calls the Relay Menu  in RLV   
`restrictions`  calls the Restrictions Menu   
`rlv`  calls the main RLV Menu   
`settings` calls the Settings Menu 

### Submenus:
`pose` calls the pose menu in Animations   
`couples`  calls the couples menu in Animations   
   
`leash configure`  calls the leash configuration menu in Leash  

`customize`  calls the Customize menu in Restrictions   
`menu managecamera` and `menu managecamera2` call the camera control menus in Restrictions > Customize   
`menu managechat` calls the muffle menu in Restrictions > Customize   
`sit` calls the menu to pick a target for force sit in the RLV menu     
`advanced` calls the Advanced menu in Restrictions   

#### Clothing/attachments:
`undress`  calls the undress menu in Apps   
`detach` or `menu detach` calls the Detach menu in Apps   
`outfits` or `menu outfits` calls the Outfits menu in Apps   
`folders`  calls the Folders menu in RLV   

#### Apps menus:
appearance - open main resizer menu
badwords -  opens badwords menu
themes  - opens themes menu
menu Capture - open capture menu
menu bell  - open bell menu
tp  - open bookmarks menu
titler / menu titler - shows menu
label / menu label  - open label menu
timer / menu timer  - open timer menu


==GENERAL FUNCTIONS==

lock - lock collar
unlock - unlock collar

fix - fix menus (will cause collar to reboot)
update - search for updater and start update process
help  - receive help notecard & link to website
touchnotify - toggle notification of collar touches on/off
allowhide - toggle allowing collar wearer to hide collar on/off
channel (number) - changes the listen channel to (number) (default is 1).
getauth - find out your access level
print auth - lists all users auth levels (owners, trusted, block) etc.
info - prints channel, safeword, prefix and collar version.
reboot - reboots collar

prefix - discover current prefix
prefix (string) - sets prefix to (string)
prefix reset - sets prefix to default (first two letters of name)

(safeword) - Safewords the collar, freeing wearer from restrictions.
safeword - print current safeword or tell if safeword is disabled
safeword off - disable safeword
safeword (word) - set safeword to (word) and enable if disabled.

runaway - start runaway process to remove all owners/trusted/block

weld - start weld process

name (string) - set name of collar wearer to (string)
name  - print name of collar wearer
device  name (string) - set name of collar to (string)
device name - print current name

print settings  - prints out all stored settings
load - loads settings from .settings notecard
load url (url)  - loads settings from a web page

==ADDING OR REMOVING OWNERS, ETC.==

add owner / add trust / add block - Open picker to add to owner / trust /block lists
rem owner / rem trust / rem block - Open picker to remove from owner / trust / block list
add owner (uuid) / add trust (uuid) / add block (uuid) - add person to list by key
rem owner (uuid) / rem trust (uuid) /rem block (uuid)  - remove person from list by key

==ANIMATION==
(anim name) - play animation
stop  / release -  stop animation
up / down - move pose offset up or down
standoffset on / standoffset off - switch offsets for standing (no pose playing) on or off
animlock  - toggle animlock on or off
posture on / posture off - switch posture collar anim (stiff neck) on or off
(couple anim name) - command wearer to do couple animation with command issuer
(couple anim name) (name) - command wearer to do couple animation with person nearby who's name matches (name)
stop couples  - stop playing couple animation
couples verbose on / couples verbose off - toggle verbose chat for couple animations on or off

==LEASHING==

yank / beckon - Pull wearer closer, unseating them if seated if they are leashed.
grab / leash - take leash
post / anchor - open menu to select object to leash wearer to 
anchor (uuid) - leash wearer to object with key uuid
follow me - make collar wearer follow command issuer
follow (uuid) - make collar wearer follow (uuid)
follow - open picker for who to follow
unleash / unfollow  - stop leashing / following
stay - disallow movement without being pulled by leash
unstay / move - allow movement again after stay has been issued
strict on / strict off - turn leash strict mode on or off
turn on / turn off - turn turn mode (leashee faces direction of movement) on or off
pass - open menu to pick person to pass leash to
pass (uuid) pass leash to (uuid) where UUID can be a person or object
length - open leash length menu
length (val) - set length of leash to val where val is a whole number from 1-60
give holder - gives a leash holder to command issuer
particle reset - reset leash settings

==CLOTHES/ATTACHMENTS==

-(string) - remove first #RLV folder found  with name that matches (string)
-- (string) - remove first #RLV folder found  with name that matches (string) and all subfolders
+(string) - Wear first #RLV folder found with name that matches (string)
&(string) - Add first #RLV folder found with name that matches (string)
++(string) - Add first #RLV folder found with name that matches (string)
&&(string) - Add first #RLV folder found with name that matches (string) and subfolders
(NOTE! We seem to have an inconsistency here where ++ does a non-recursive (no subfolder) add rather than a recursive wear.)

wear - Open list of outfits to wear
wear (outfit) - wear outfit called (outfit)
naked - remove all outfits (and everything outside .core if strip all mode is on

undress lock (layer) - locks a clothing layer (layer)
undress unlock (layer) - unlocks a clothing layer (layer)

detach - Open list of attachments to remove

RLV RESTRICTIONS/EXCEPTIONS & FUNCTIONS

rlv on / rlv off - switches RLV functions in the collar on or off. 
clear - clears all RLV.

relay off / relay ask / relay auto - set relay mode
relay helpless - toggle helpless mode on / off
relay wearer - toggle wearer lockout for relay options

rlv handshakes (number) - sets the number of times the collar will attempt to confirm RLV is active in the viewer. Default is 3 and if this isn't enough there's probably something badly wrong with your connection, but you can increase it here if your collar is not recognizing RLV on attach / logon.

show restrictions  -  list all restrictions from all sources that are handled by the collar (for example, including relay restrictions
list presets - shows current restriction presets and what they do. Default presets are Hear, Talk, Touch, Stray, Inventory, Dress, IM, Names/Map and Blur, but these can be changed  via the [Customize] submenu in Restrictions. These can be set or cleared using the commands below, replacing (preset) with the name of the preset you wish to add or remove. Note that these are case sensitive (i.e you have to use "Blur" rather than "blur").
preset add (preset) - activates preset (preset).
preset replace (preset) - removes current presets and adds (preset) as new restriction set
preset clear (preset) - removes preset (preset)

garble on - activates garbling when talk restriction is set
garble off - deactivates garbling

sit (uuid) - force sit on object with key (uuid)
unsit - force wearer to stand

rlv list - lists all current restrictions
rlv add (restriction) - adds individual restriction (see below)
rlv rem (restriction) - removes individual restricion (see below)

INDIVIDUAL RESTRICTIONS:
The following individual restrictions can be added or cleared with the above commands, using either the prettified button name for the restriction or its actual internal RLV command. Note that where a command requires a value (such as the camera max distance) it will apply the value that has been set in the relevant configuration menus. For more information on what each command does, consult the RLV API document at https://wiki.secondlife.com/wiki/LSL_Protocol/RestrainedLoveAPI and look up the individual internal command.

Button command   =  internal RLV command
------------------------------------------------------
    EmoteTrunc    =    emote
    Send Chat    =    sendchat
    See Chat    =    recvchat
    See Emote    =    recvemote
    Whisper    =    chatwhisper
    Normal Chat    =    chatnormal
    Shout    =    chatshout
    Send IM    =    sendim
    See IM    =    recvim
    Start IM    =    startim
    Gesture    =    sendgesture
    Inventory    =    showinv
    Minimap    =    showminimap
    Worldmap    =    showworldmap
    Location    =    showloc
    Names    =    shownames
    Nametags    =    shownametags
    Nearby    =    shownearby
    Text    =    showhovertext
    Text HUD    =    showhovertexthud
    Text World    =    showhovertextworld
    Text All    =    showhovertextall
    Landmark    =    tplm
    TP Location    =    tploc
    TP Local    =    tplocal
    Accept TP    =    tplure
    Offer TP    =    prequest
    Permissions    =    acceptpermission
    Edit    =    edit
    Edit Object    =    editobj
    Rez"    =    rez
    Add Attach    =    "addattach
    Rem Attach    =    remattach
    Add Cloth    =    addoutfit
    Rem Cloth    =    remoutfit
    Notecard    =    viewnote
    Script    =    viewscript
    Texture    =    viewtexture
    Touch Far    =    fartouch
    Interact    =    interact
    Attachment    =    touchattach
    Own Attach    =    touchattachself
    Other Attach    =    touchattachother
    Touch HUD    =    touchhud
    Touch World    =    touchworld
    Touch All    =    touchall
    Fly    =    fly
    Jump    =    jump
    Stand Up    =    unsit
    Sit Down    =    sit
    Sit TP    =    sittp
    Stand TP    =    standtp
    Always Run    =    alwaysrun
    Temp Run    =    temprun
    Unlock Cam    =    camunlock
    Blur View    =    setdebug_renderresolutiondivisor
    MaxDistance    =    setcam_avdistmax
    MinDistance    =    setcam_avdistmin
    Send Emote    =    rediremote
    Set Debug    =    setdebug
    Environment    =    setenv
    Mouselook    =    camdistmax:0
    
EXAMPLE: "/1 (prefix) rlv add fly"


[Exceptions stuff -- experts only!]
rlvex modify owner (val) / rlvex modify trust (val) - sets owner and trust exceptions to (val) where (val) is the bitmask of exceptions
rlvex modify (custom) (val) - as above but changes custom value
rlvex listmasks - lists  bitmasks values
rlvex help  - lists valid commands for changing bitmasks
rlvex listcustom - lists custom exceptions and their bitmasks



==APPS==

BELL
bell volume (number from 1-10) set bell volume
bell on / bell off - turn bell on or off
bell nextsound - changes to next available sound for bell noise
bell ring - rings the bell once
rm bell - Uninstall bell script.

BOOKMARKS
tp save - open dialog to save current location
tp save (name) - create bookmark called (name) to current location
tp remove - open list of bookmarks to remove
tp remove (name) - remove bookmark called (name)
tp (name) - tp wearer to location of bookmark called (name)
rm bookmarks - uninstall bookmark app

LABEL/MESHLABEL
label font - open font picker menu
label font (name) - set font to (name). Default values are "Andale 1", "Andale 2", "Serif 1", "Serif 2", "LCD".
label color (vector) - sets label color to (vector) - i.e <1,1,1> for white
label on - show label
label off - hide label
label scroll on - scroll label text
label scroll off - stop scrolling
label (text) - set label to (text)
rm label - uninstall label app

RESIZER
rotation - open rotation menu
position - open position menu
size - open size menu
rm resizer  - uninstall resizer app

THEMES
newtheme - lists current properties to save into a new theme notecard
hide - sets collar invisible
show - unhides collar

TITLER
title  - opens textbox to type in new title
title (text) / titler title (text) - sets title to (text)
titler color - opens color menu
titler color (vector) - sets title color to (vector)
titler show - shows title
titler hide - hides title
titler up - moves title higher
titler down - moves title lower
titler plain  - toggles plaintext mode that saves title as either plaintext or base64 encoded

BADWORDS
badwords add - opens text box to enter new phrase to add to bad words list
badwords add (phrase) - adds (phrase) to bad words list
badwords animation (anim) - sets the animation to trigger when a bad word is spoken
badwords animation default - restores animation to the default shock animation
badwords sound (name) - changes the sound triggered when a bad word is spoken to (name)
badwords sound silent - disables badword sounds
badwords penance - open textbox to add new penance phrase
badwords penance (phrase) - change the penance phrase to (phrase)
badwords remove - open list of badwords to remove
badwords remove (phrase) - removes (phrase) from badwords list
badwords on / badwords off - switch on or off
badwords clear - clear all bad words from list

CAPTURE
capture dump - print capture status
capture on - activate capture mode
capture off - deactivate capture mode
capture - attempt to capture

TIMER
timer permissive on / timer permissive off - set timer permissive mode on or off
timer endnow - end active timer instantly
timer cancel  - cancels active timer, does not issue end of timer commands
timer start - starts timer
timer time -  opens time menu
timer time (time) - sets timer to (time), where (time) is in hours, minutes and seconds (e.g 2hrs 10m). Function will read most sensible ways of writing time, don't worry.
timer customs - opens text box to add custom commands (a list of chat commands separated by commas) that will be issued when timer expires
timer customs (commands) - sets (commands) as a comma separated list of chat commands that will be issued when timer expires
timer lockout on / timer lockout off - switches wearer lockout while timer active on or off
timer unleash on / timer unleash off - switches unleash when timer expires on or off
timer unpose on / timer unpose off - switches ending poses when timer expires on or off
timer clearrlv on / timer clearrlv off - switches clearing rlv restrictions when timer expires on or off
timer unsit on / timer unsit off - switches unsitting collar wearer when timer expires on or off
timer titler on / timer titler off  - switches time left titler on or off

CAGEHOME
ch here  -sets current location as cagehome "cage"
ch arm  - activates cage home, with setter marked as primary
ch disarm - deactivates cagehome if armed but sub not caged
ch release - release sub
ch settings - list cagehome settings
ch commands - list cagehome chat commands
ch warntime <seconds> - amount of time before caging where sub is given warning it's about to happen
ch radius <meters> - distance sub can move from "cage" location
ch cagetime <minutes> - timer for caging. At 0, there's no timer.
ch notifychannel <channel number> - sends notification on specified channel on capture and release (will not use channel 0).
ch notifyarrive <arrive string> - phrase said on capture
ch notifyrelease <release string> - phrase said on release
ch warnmessage <warning message> - phrase in local chat said when sub is being summoned. "@" will be replaced by sub's name. # will be replaced by number of seconds of cagetime set.