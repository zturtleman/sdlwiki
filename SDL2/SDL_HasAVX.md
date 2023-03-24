###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_HasAVX

Determine whether the CPU has AVX features.

## Syntax

```c
SDL_bool SDL_HasAVX(void);

```

## Return Value

Returns [SDL_TRUE](SDL_TRUE) if the CPU has AVX features or
[SDL_FALSE](SDL_FALSE) if not.

## Remarks

This always returns false on CPUs that aren't using Intel instruction sets.

## Version

This function is available since SDL 2.0.2.

## Related Functions

* [SDL_Has3DNow](SDL_Has3DNow)
* [SDL_HasAltiVec](SDL_HasAltiVec)
* [SDL_HasAVX2](SDL_HasAVX2)
* [SDL_HasMMX](SDL_HasMMX)
* [SDL_HasRDTSC](SDL_HasRDTSC)
* [SDL_HasSSE](SDL_HasSSE)
* [SDL_HasSSE2](SDL_HasSSE2)
* [SDL_HasSSE3](SDL_HasSSE3)
* [SDL_HasSSE41](SDL_HasSSE41)
* [SDL_HasSSE42](SDL_HasSSE42)

----
[CategoryAPI](CategoryAPI), [CategoryCPU](CategoryCPU)


