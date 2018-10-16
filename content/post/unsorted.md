+++
title = "unsorted"
topics = []
keywords = ["osx"]
description = "unsorted stuff"
draft = false
type = "post"
date = "2017-01-10T13:58:52+01:00"
tags = ["osx", "tmux"]
author = "Börje Granberg"

+++

### Hackingtosh
Installationsguide: https://www.tonymacx86.com/threads/how-to-install-os-x-yosemite-using-clover.144426/

### Audio in OXS 10.12 Sierra

This work with Clover https://github.com/toleda/audio_CloverALC/blob/master/audio_cloverALC-120.command.zip

### Numpad i iterm2
http://superuser.com/questions/565178/how-do-i-get-the-numpad-to-work-in-vim-using-iterm2-on-osx-with-term-xterm
Preferences->Profiles->Keys and load preset of: "xterm with Numeric Keypad".
### Home & End keys in OSX
http://www.jvandemo.com/how-to-fix-home-and-end-keys-on-mac-os-x/
```
$ cd ~/Library
$ mkdir KeyBindings
$ cd KeyBindings
$ vi DefaultKeyBinding.dict

```
Copy/paste the following lines:

```
{
/* Remap Home / End keys to be correct */
"\UF729" = "moveToBeginningOfLine:"; /* Home */
"\UF72B" = "moveToEndOfLine:"; /* End */
"$\UF729" = "moveToBeginningOfLineAndModifySelection:"; /* Shift + Home */
"$\UF72B" = "moveToEndOfLineAndModifySelection:"; /* Shift + End */
"^\UF729" = "moveToBeginningOfDocument:"; /* Ctrl + Home */
"^\UF72B" = "moveToEndOfDocument:"; /* Ctrl + End */
"$^\UF729" = "moveToBeginningOfDocumentAndModifySelection:"; /* Shift + Ctrl + Home */
"$^\UF72B" = "moveToEndOfDocumentAndModifySelection:"; /* Shift + Ctrl + End */
}
```

### USB unmounts during write/read

Follow this suggestion: https://www.tonymacx86.com/threads/how-to-get-usb-3-0-working-on-ga-z68mx-ud2h-b3.176326/page-3#post-1280629

I Removed  FakePCIID_XHCIMux.kext & FakePCIID.kext from /S/L/E

----

Removed GenericUSHXHCI from /L/E
Using Multibeast 9.2.1 reinstalled 7/8/9 Series USB Support (and then got new Fake*.kexts)
 
