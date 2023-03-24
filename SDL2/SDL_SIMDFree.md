###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_SIMDFree

Deallocate memory obtained from [SDL_SIMDAlloc](SDL_SIMDAlloc) 

## Syntax

```c
void SDL_SIMDFree(void *ptr);

```

## Function Parameters

|             |                                                                                                                                        |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **ptr**     | The pointer, returned from [SDL_SIMDAlloc](SDL_SIMDAlloc) or [SDL_SIMDRealloc](SDL_SIMDRealloc), to deallocate. NULL is a legal no-op. |

## Remarks

It is not valid to use this function on a pointer from anything but
[SDL_SIMDAlloc](SDL_SIMDAlloc)() or [SDL_SIMDRealloc](SDL_SIMDRealloc)().
It can't be used on pointers from malloc, realloc,
[SDL_malloc](SDL_malloc), memalign, new[], etc.

However, [SDL_SIMDFree](SDL_SIMDFree)(NULL) is a legal no-op.

The memory pointed to by `ptr` is no longer valid for access upon return,
and may be returned to the system or reused by a future allocation. The
pointer passed to this function is no longer safe to dereference once this
function returns, and should be discarded.

## Version

This function is available since SDL 2.0.10.

## Related Functions

* [SDL_SIMDAlloc](SDL_SIMDAlloc)
* [SDL_SIMDRealloc](SDL_SIMDRealloc)

----
[CategoryAPI](CategoryAPI), [CategoryCPU](CategoryCPU)


