# CategoryJoystick

SDL joystick support.

This is the lower-level joystick handling. If you want the simpler option,
where what buttons does what is well-defined, you should use the gamepad
API instead.

The term "instance_id" is the current instantiation of a joystick device in
the system, if the joystick is removed and then re-inserted then it will
get a new instance_id, instance_id's are monotonically increasing
identifiers of a joystick plugged in.

The term "player_index" is the number assigned to a player on a specific
controller. For XInput controllers this returns the XInput user index. Many
joysticks will not be able to supply this information.

The term [SDL_JoystickGUID](SDL_JoystickGUID) is a stable 128-bit
identifier for a joystick device that does not change over time, it
identifies class of the device (a X360 wired controller for example). This
identifier is platform dependent.

In order to use these functions, [SDL_Init](SDL_Init)() must have been
called with the [SDL_INIT_JOYSTICK](SDL_INIT_JOYSTICK) flag. This causes
SDL to scan the system for joysticks, and load appropriate drivers.

If you would like to receive joystick updates while the application is in
the background, you should set the following hint before calling
[SDL_Init](SDL_Init)():
[SDL_HINT_JOYSTICK_ALLOW_BACKGROUND_EVENTS](SDL_HINT_JOYSTICK_ALLOW_BACKGROUND_EVENTS)

<!-- END CATEGORY DOCUMENTATION -->

## Functions

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryJoystick, CategoryAPIFunction -->
- [SDL_AttachVirtualJoystick](SDL_AttachVirtualJoystick)
- [SDL_CloseJoystick](SDL_CloseJoystick)
- [SDL_DetachVirtualJoystick](SDL_DetachVirtualJoystick)
- [SDL_GetJoystickAxis](SDL_GetJoystickAxis)
- [SDL_GetJoystickAxisInitialState](SDL_GetJoystickAxisInitialState)
- [SDL_GetJoystickBall](SDL_GetJoystickBall)
- [SDL_GetJoystickButton](SDL_GetJoystickButton)
- [SDL_GetJoystickConnectionState](SDL_GetJoystickConnectionState)
- [SDL_GetJoystickFirmwareVersion](SDL_GetJoystickFirmwareVersion)
- [SDL_GetJoystickFromInstanceID](SDL_GetJoystickFromInstanceID)
- [SDL_GetJoystickFromPlayerIndex](SDL_GetJoystickFromPlayerIndex)
- [SDL_GetJoystickGUID](SDL_GetJoystickGUID)
- [SDL_GetJoystickGUIDFromString](SDL_GetJoystickGUIDFromString)
- [SDL_GetJoystickGUIDInfo](SDL_GetJoystickGUIDInfo)
- [SDL_GetJoystickGUIDString](SDL_GetJoystickGUIDString)
- [SDL_GetJoystickHat](SDL_GetJoystickHat)
- [SDL_GetJoystickInstanceGUID](SDL_GetJoystickInstanceGUID)
- [SDL_GetJoystickInstanceID](SDL_GetJoystickInstanceID)
- [SDL_GetJoystickInstanceName](SDL_GetJoystickInstanceName)
- [SDL_GetJoystickInstancePath](SDL_GetJoystickInstancePath)
- [SDL_GetJoystickInstancePlayerIndex](SDL_GetJoystickInstancePlayerIndex)
- [SDL_GetJoystickInstanceProduct](SDL_GetJoystickInstanceProduct)
- [SDL_GetJoystickInstanceProductVersion](SDL_GetJoystickInstanceProductVersion)
- [SDL_GetJoystickInstanceType](SDL_GetJoystickInstanceType)
- [SDL_GetJoystickInstanceVendor](SDL_GetJoystickInstanceVendor)
- [SDL_GetJoystickName](SDL_GetJoystickName)
- [SDL_GetJoystickPath](SDL_GetJoystickPath)
- [SDL_GetJoystickPlayerIndex](SDL_GetJoystickPlayerIndex)
- [SDL_GetJoystickPowerInfo](SDL_GetJoystickPowerInfo)
- [SDL_GetJoystickProduct](SDL_GetJoystickProduct)
- [SDL_GetJoystickProductVersion](SDL_GetJoystickProductVersion)
- [SDL_GetJoystickProperties](SDL_GetJoystickProperties)
- [SDL_GetJoysticks](SDL_GetJoysticks)
- [SDL_GetJoystickSerial](SDL_GetJoystickSerial)
- [SDL_GetJoystickType](SDL_GetJoystickType)
- [SDL_GetJoystickVendor](SDL_GetJoystickVendor)
- [SDL_GetNumJoystickAxes](SDL_GetNumJoystickAxes)
- [SDL_GetNumJoystickBalls](SDL_GetNumJoystickBalls)
- [SDL_GetNumJoystickButtons](SDL_GetNumJoystickButtons)
- [SDL_GetNumJoystickHats](SDL_GetNumJoystickHats)
- [SDL_HasJoystick](SDL_HasJoystick)
- [SDL_IsJoystickVirtual](SDL_IsJoystickVirtual)
- [SDL_JoystickConnected](SDL_JoystickConnected)
- [SDL_JoystickEventsEnabled](SDL_JoystickEventsEnabled)
- [SDL_LockJoysticks](SDL_LockJoysticks)
- [SDL_OpenJoystick](SDL_OpenJoystick)
- [SDL_RumbleJoystick](SDL_RumbleJoystick)
- [SDL_RumbleJoystickTriggers](SDL_RumbleJoystickTriggers)
- [SDL_SendJoystickEffect](SDL_SendJoystickEffect)
- [SDL_SendJoystickVirtualSensorData](SDL_SendJoystickVirtualSensorData)
- [SDL_SetJoystickEventsEnabled](SDL_SetJoystickEventsEnabled)
- [SDL_SetJoystickLED](SDL_SetJoystickLED)
- [SDL_SetJoystickPlayerIndex](SDL_SetJoystickPlayerIndex)
- [SDL_SetJoystickVirtualAxis](SDL_SetJoystickVirtualAxis)
- [SDL_SetJoystickVirtualBall](SDL_SetJoystickVirtualBall)
- [SDL_SetJoystickVirtualButton](SDL_SetJoystickVirtualButton)
- [SDL_SetJoystickVirtualHat](SDL_SetJoystickVirtualHat)
- [SDL_SetJoystickVirtualTouchpad](SDL_SetJoystickVirtualTouchpad)
- [SDL_UnlockJoysticks](SDL_UnlockJoysticks)
- [SDL_UpdateJoysticks](SDL_UpdateJoysticks)
<!-- END CATEGORY LIST -->

## Datatypes

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryJoystick, CategoryAPIDatatype -->
- [SDL_JoystickGUID](SDL_JoystickGUID)
- [SDL_JoystickID](SDL_JoystickID)
<!-- END CATEGORY LIST -->

## Structs

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryJoystick, CategoryAPIStruct -->
- [SDL_Joystick](SDL_Joystick)
- [SDL_VirtualJoystickDesc](SDL_VirtualJoystickDesc)
- [SDL_VirtualJoystickSensorDesc](SDL_VirtualJoystickSensorDesc)
- [SDL_VirtualJoystickTouchpadDesc](SDL_VirtualJoystickTouchpadDesc)
<!-- END CATEGORY LIST -->

## Enums

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryJoystick, CategoryAPIEnum -->
- [SDL_JoystickConnectionState](SDL_JoystickConnectionState)
- [SDL_JoystickType](SDL_JoystickType)
<!-- END CATEGORY LIST -->

## Macros

<!-- DO NOT HAND-EDIT CATEGORY LISTS, THEY ARE AUTOGENERATED AND WILL BE OVERWRITTEN, BASED ON TAGS IN INDIVIDUAL PAGE FOOTERS. EDIT THOSE INSTEAD. -->
<!-- BEGIN CATEGORY LIST: CategoryJoystick, CategoryAPIMacro -->
- [SDL_JOYSTICK_AXIS_MAX](SDL_JOYSTICK_AXIS_MAX)
- [SDL_JOYSTICK_AXIS_MIN](SDL_JOYSTICK_AXIS_MIN)
<!-- END CATEGORY LIST -->


----
[CategoryAPICategory](CategoryAPICategory)


