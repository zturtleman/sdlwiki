###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_CreateSemaphore

Create a semaphore.

## Syntax

```c
SDL_sem* SDL_CreateSemaphore(Uint32 initial_value);

```

## Function Parameters

|                       |                                     |
| --------------------- | ----------------------------------- |
| **initial_value**     | the starting value of the semaphore |

## Return Value

Returns a new semaphore or NULL on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function creates a new semaphore and initializes it with the value
`initial_value`. Each wait operation on the semaphore will atomically
decrement the semaphore value and potentially block if the semaphore value
is 0. Each post operation will atomically increment the semaphore value and
wake waiting threads and allow them to retry the wait operation.

## Version

This function is available since SDL 3.0.0.

## Code Examples

<!-- # Begin Semaphore Example -->
Typical use of semaphores:
```c++
SDL_atomic_t done;
SDL_sem *sem;

SDL_AtomicSet(&done, 0);
sem = SDL_CreateSemaphore(0);
.
.
Thread A:
    while (!SDL_AtomicGet(&done)) {
        add_data_to_queue();
        SDL_SemPost(sem);
    }

Thread B:
    while (!SDL_AtomicGet(&done)) {
        SDL_SemWait(sem);
        if (data_available()) {
            get_data_from_queue();
        }
    }
.
.
SDL_AtomicSet(&done, 1);
SDL_SemPost(sem);
wait_for_threads();
SDL_DestroySemaphore(sem);
```
<!-- # End Semaphore Example -->

## Related Functions

* [SDL_DestroySemaphore](SDL_DestroySemaphore)
* [SDL_SemPost](SDL_SemPost)
* [SDL_SemTryWait](SDL_SemTryWait)
* [SDL_SemValue](SDL_SemValue)
* [SDL_SemWait](SDL_SemWait)
* [SDL_SemWaitTimeout](SDL_SemWaitTimeout)

----
[CategoryAPI](CategoryAPI), [CategoryMutex](CategoryMutex)

