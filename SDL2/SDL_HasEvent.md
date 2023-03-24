###### (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)
# SDL_HasEvent

Check for the existence of a certain event type in the event queue.

## Syntax

```c
SDL_bool SDL_HasEvent(Uint32 type);

```

## Function Parameters

|              |                                                                                 |
| ------------ | ------------------------------------------------------------------------------- |
| **type**     | the type of event to be queried; see [SDL_EventType](SDL_EventType) for details |

## Return Value

Returns [SDL_TRUE](SDL_TRUE) if events matching `type` are present, or
[SDL_FALSE](SDL_FALSE) if events matching `type` are not present.

## Remarks

If you need to check for a range of event types, use
[SDL_HasEvents](SDL_HasEvents)() instead.

## Version

This function is available since SDL 2.0.0.

## Related Functions

* [SDL_HasEvents](SDL_HasEvents)

----
[CategoryAPI](CategoryAPI), [CategoryEvents](CategoryEvents)


