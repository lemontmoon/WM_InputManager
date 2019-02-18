# WM_InputManager

Overview :

Realtime visual RAWINPUT/XINPUT USB Device Manager. You can use any HID-Compliant Gamepads/Joysticks as your input device with the ability to visually use, remap, configure, debug, assign device to specific a player (PlayerController) during gameplay with pre-built UMG menus included in package.

It detects controllers with visual events Plug&Play functionality implemented inside the manager. All Devices have their own memory which memorizes 2 device modes that the developer or player can configure during gameplay.

If your device is plugged in it will automatically list your device in WM_InputManagerUMG & will read all possible inputs and give you an options list for you to easily remap or configure.

Each WM_Controller Input key will list all ACTIONS in which they are used.

Each device will automatically autodetect axis type on first connected. Detects if axes are pedals 0-1 range or -1 1 or inverted. Configure , sensitivity, deadzone with magnitude, "Auto/Reset" button for axes.

You can make your own visual templates for SteeringWheel , FlightStick etc.

ManagerUMG will list for you all used WM_Controller input keys with corresponding bound actions & combo options to pick target input path you wish.

WM_InputUMG must be added to Viewport inside GameMode because you have global control over devices while configuring so don't do that in PlayerController if you are creating more local players.

It is a perfect solution for Local Multiplayer Games to allow players to quickly assign device to specific a PlayerController.


Features:
players & developers can remap Device Input paths visually during gameplay(shipping = OK)
All Devices has 2 configuration modes saved in memmory using savefiles and folder (Saved/WMDeviceConfigurations/)
Each Gaming controller has predefined setup which will work for most of gamepads avaliable
Easy button remapping with just one click (HOLD&Press)
automatic Axis type detection when device is 1stTime connected or via "Auto/Reset" (will detect if you have pedals 0-1 axis)
"LISTEN" for input
PlayerController device assigment (via widget for assigning controller with dpad controlls or arrow clicks)
Use multiple devices per player & combine their input (virtually build multicontroller)
Perfect for game which is designed for more local players on one computer (Combat games, cooperative, fight)
Sensitivity, DeadZone, Invert, isPedal config
no need for XInput & other device emulators.
