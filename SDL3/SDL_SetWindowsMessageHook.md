###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)

## Draft

**THIS PAGE IS A WORK IN PROGRESS** ... Please make edits to this page to improve it!


<!-- #*^*^*^*^*See https://wiki.libsdl.org/SGFunctions for details on editing this page*^*^*^*^* -->
# SDL_SetWindowsMessageHook

Set a callback for every Windows message, run before TranslateMessage().

## Syntax

```c
void SDL_SetWindowsMessageHook(SDL_WindowsMessageHook callback, void *userdata);

```

## Function Parameters

|                  |                                                                        |
| ---------------- | ---------------------------------------------------------------------- |
| **callback**     | The [SDL_WindowsMessageHook](SDL_WindowsMessageHook) function to call. |
| **userdata**     | a pointer to pass to every iteration of `callback`                     |

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategorySystem](CategorySystem), [CategoryDraft](CategoryDraft)
<!-- #See the Style Guide for instructions on editing the footer. -->


