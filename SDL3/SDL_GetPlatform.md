###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_GetPlatform

Get the name of the platform.

## Header File

Defined in [<SDL3/SDL_platform.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_platform.h)

## Syntax

```c
const char * SDL_GetPlatform(void);
```

## Return Value

Returns the name of the platform. If the correct platform name is not
available, returns a string beginning with the text "Unknown".

## Remarks

Here are the names returned for some (but not all) supported platforms:

- "Windows"
- "macOS"
- "Linux"
- "iOS"
- "Android"

The returned string follows the [SDL_GetStringRule](SDL_GetStringRule).

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPlatform](CategoryPlatform)

