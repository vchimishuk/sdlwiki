###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_OpenJoystick

Open a joystick for use.

## Header File

Defined in [<SDL3/SDL_joystick.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_joystick.h)

## Syntax

```c
SDL_Joystick* SDL_OpenJoystick(SDL_JoystickID instance_id);
```

## Function Parameters

|                     |                          |
| ------------------- | ------------------------ |
| **instance_id**     | the joystick instance ID |

## Return Value

Returns a joystick identifier or NULL if an error occurred; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The joystick subsystem must be initialized before a joystick can be opened
for use.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_CloseJoystick](SDL_CloseJoystick)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

