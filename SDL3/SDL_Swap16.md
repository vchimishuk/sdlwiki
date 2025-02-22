###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_Swap16

Byte-swap an unsigned 16-bit number.

## Header File

Defined in [<SDL3/SDL_endian.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_endian.h)

## Syntax

```c
SDL_FORCE_INLINE Uint16 SDL_Swap16(Uint16 x);
```

## Function Parameters

|           |                         |
| --------- | ----------------------- |
| **x**     | the value to byte-swap. |

## Return Value

Returns `x`, with its bytes in the opposite endian order.

## Remarks

This will always byte-swap the value, whether it's currently in the native
byteorder of the system or not. You should use [SDL_Swap16LE](SDL_Swap16LE)
or [SDL_Swap16BE](SDL_Swap16BE) instead, in most cases.

Note that this is a forced-inline function in a header, and not a public
API function available in the SDL library (which is to say, the code is
embedded in the calling program and the linker and dynamic loader will not
be able to find this function inside SDL itself).

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryEndian](CategoryEndian)

