---
title: How to disable a key from the keyboard on Windows?
layout: post
categories:
- Windows
image: assets/images/keyboard.jpeg
description: |-
  In this blog post we will give a step by step process to diasble a key from keyboard on your microsoft windows Operating suste,

  here's a step-by-step guide on how to disable a key from the keyboard on Windows:
---

Image Source: wikihow

In this blog post we will give a step by step process to diasble a key from keyboard on your microsoft windows Operating suste,

here's a step-by-step guide on how to disable a key from the keyboard on Windows:

1. Open the Registry Editor: To do this, press Windows Key + R on your keyboard to open the Run dialog box. Type "regedit" (without the quotes) and press Enter. If prompted for permission, click "Yes".

2. Navigate to the Keyboard Layout key: In the Registry Editor, navigate to the following key: HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout

3. Create a new Binary Value: Right-click on the Keyboard Layout key and select New > Binary Value. Name the new value "Scancode Map" (without the quotes).
![]({{ 'assets/images/keyboard2.jpg' | relative_url }})

4. Edit the Scancode Map value: Double-click on the Scancode Map value to edit it. In the "Value data" field, enter the following hex code: 00 00 00 00 00 00 00 00 03 00 00 00 00 00 2a e0 00 00 37 e0 00 00 00 00. 
Note: This hex code disables the "Caps Lock" key. If you want to disable a different key, you'll need to find its scan code and modify the hex code accordingly.

5. Save and exit the Registry Editor: Click OK to save the Scancode Map value and exit the Registry Editor.

6.Restart your computer: This step is important to ensure that the changes you made take effect.

And that's it! The key you disabled should no longer work on your keyboard. If you ever want to re-enable the key, simply go back into the Registry Editor and delete the Scancode Map value.
