###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_GetGamepadTouchpadFinger

Get the current state of a finger on a touchpad on a gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
int SDL_GetGamepadTouchpadFinger(SDL_Gamepad *gamepad, int touchpad, int finger, Uint8 *state, float *x, float *y, float *pressure);
```

## Function Parameters

|                  |                                                                              |
| ---------------- | ---------------------------------------------------------------------------- |
| **gamepad**      | a gamepad                                                                    |
| **touchpad**     | a touchpad                                                                   |
| **finger**       | a finger                                                                     |
| **state**        | filled with state                                                            |
| **x**            | filled with x position, normalized 0 to 1, with the origin in the upper left |
| **y**            | filled with y position, normalized 0 to 1, with the origin in the upper left |
| **pressure**     | filled with pressure value                                                   |

## Return Value

Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetNumGamepadTouchpadFingers](SDL_GetNumGamepadTouchpadFingers)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

