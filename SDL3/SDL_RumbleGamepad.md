###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_RumbleGamepad

Start a rumble effect on a gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
int SDL_RumbleGamepad(SDL_Gamepad *gamepad, Uint16 low_frequency_rumble, Uint16 high_frequency_rumble, Uint32 duration_ms);
```

## Function Parameters

|                               |                                                                            |
| ----------------------------- | -------------------------------------------------------------------------- |
| **gamepad**                   | The gamepad to vibrate                                                     |
| **low_frequency_rumble**      | The intensity of the low frequency (left) rumble motor, from 0 to 0xFFFF   |
| **high_frequency_rumble**     | The intensity of the high frequency (right) rumble motor, from 0 to 0xFFFF |
| **duration_ms**               | The duration of the rumble effect, in milliseconds                         |

## Return Value

Returns 0, or -1 if rumble isn't supported on this gamepad

## Remarks

Each call to this function cancels any previous rumble effect, and calling
it with 0 intensity stops any rumbling.

This function requires you to process SDL events or call
[SDL_UpdateJoysticks](SDL_UpdateJoysticks)() to update rumble state.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

