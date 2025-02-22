###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_GetTouchDeviceName

Get the touch device name as reported from the driver.

## Header File

Defined in [<SDL3/SDL_touch.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_touch.h)

## Syntax

```c
const char* SDL_GetTouchDeviceName(SDL_TouchID touchID);
```

## Function Parameters

|                 |                               |
| --------------- | ----------------------------- |
| **touchID**     | the touch device instance ID. |

## Return Value

Returns touch device name, or NULL on error; call
[SDL_GetError](SDL_GetError)() for more details.

## Remarks

The returned string follows the [SDL_GetStringRule](SDL_GetStringRule).

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryTouch](CategoryTouch)

