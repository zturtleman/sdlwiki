
# Thread Synchronization Primitives

'''Include File(s):'''  [http://hg.libsdl.org/SDL/file/default/include/SDL_mutex.h SDL_mutex.h], [http://hg.libsdl.org/SDL/file/default/include/SDL_thread.h SDL_thread.h]


## Introduction

Functions in this group provide thread synchronization primitives for multi-threaded programing.

There are three primitives available in SDL:
* Mutex
* Semaphore
* Condition Variable

The SDL mutex is implemented as a recursive mutex so you can nest lock and unlock calls to the same mutex.


<!-- #Remove this line and the ## below to use this markup if it becomes relevant to this category -->
<!-- #== Enumerations == -->
<!-- #<<FullSearchCached(category:CategoryEnum CategoryMutex -title:SGEnumerations)>> -->

<!-- #== Structures == -->
<!-- #<<FullSearchCached(category:CategoryStruct CategoryMutex -title:SGStructures)>> -->

## Functions
<<FullSearchCached(category:CategoryMutex -CategoryEnum -CategoryStruct -title:SGFunctions)>>

<!-- BEGIN CATEGORY LIST -->
- [SDL_CondBroadcast](SDL_CondBroadcast)
- [SDL_CondSignal](SDL_CondSignal)
- [SDL_CondWait](SDL_CondWait)
- [SDL_CondWaitTimeout](SDL_CondWaitTimeout)
- [SDL_CreateCond](SDL_CreateCond)
- [SDL_CreateMutex](SDL_CreateMutex)
- [SDL_CreateSemaphore](SDL_CreateSemaphore)
- [SDL_DestroyCond](SDL_DestroyCond)
- [SDL_DestroyMutex](SDL_DestroyMutex)
- [SDL_DestroySemaphore](SDL_DestroySemaphore)
- [SDL_LockMutex](SDL_LockMutex)
- [SDL_SemPost](SDL_SemPost)
- [SDL_SemTryWait](SDL_SemTryWait)
- [SDL_SemValue](SDL_SemValue)
- [SDL_SemWait](SDL_SemWait)
- [SDL_SemWaitTimeout](SDL_SemWaitTimeout)
- [SDL_TryLockMutex](SDL_TryLockMutex)
- [SDL_UnlockMutex](SDL_UnlockMutex)
<!-- END CATEGORY LIST -->

----
[CategoryCategory](CategoryCategory)
