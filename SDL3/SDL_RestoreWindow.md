###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_RestoreWindow

Restore the size and position of a minimized or maximized window.

## Syntax

```c
int SDL_RestoreWindow(SDL_Window *window);

```

## Function Parameters

|                |                       |
| -------------- | --------------------- |
| **window**     | the window to restore |

## Return Value

Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.0.0.

## Related Functions

* [SDL_MaximizeWindow](SDL_MaximizeWindow)
* [SDL_MinimizeWindow](SDL_MinimizeWindow)

----
[CategoryAPI](CategoryAPI), [CategoryVideo](CategoryVideo)


