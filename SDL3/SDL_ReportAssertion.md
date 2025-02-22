###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_ReportAssertion

Never call this directly.

## Header File

Defined in [<SDL3/SDL_assert.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_assert.h)

## Syntax

```c
SDL_AssertState SDL_ReportAssertion(SDL_AssertData *data,
                                const char *func,
                                const char *file, int line);
```

## Function Parameters

|              |                       |
| ------------ | --------------------- |
| **data**     | assert data structure |
| **func**     | function name         |
| **file**     | file name             |
| **line**     | line number           |

## Return Value

Returns assert state

## Remarks

Use the [SDL_assert](SDL_assert)* macros instead.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAssert](CategoryAssert)

