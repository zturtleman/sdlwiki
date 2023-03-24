###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_GetCursor

Get the active cursor.

## Syntax

```c
SDL_Cursor* SDL_GetCursor(void);

```

## Return Value

Returns the active cursor or NULL if there is no mouse.

## Remarks

This function returns a pointer to the current cursor which is owned by the
library. It is not necessary to free the cursor with
[SDL_FreeCursor](SDL_FreeCursor)().

## Version

This function is available since SDL 2.0.0.

## Related Functions

* [SDL_SetCursor](SDL_SetCursor)

----
[CategoryAPI](CategoryAPI), [CategoryMouse](CategoryMouse)

