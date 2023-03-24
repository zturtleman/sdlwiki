###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_CloseAudioDevice

Use this function to shut down audio processing and close the audio device.

## Syntax

```c
void SDL_CloseAudioDevice(SDL_AudioDeviceID dev);

```

## Function Parameters

|             |                                                                                     |
| ----------- | ----------------------------------------------------------------------------------- |
| **dev**     | an audio device previously opened with [SDL_OpenAudioDevice](SDL_OpenAudioDevice)() |

## Remarks

The application should close open audio devices once they are no longer
needed. Calling this function will wait until the device's audio callback
is not running, release the audio hardware and then clean up internal
state. No further audio will play from this device once this function
returns.

This function may block briefly while pending audio data is played by the
hardware, so that applications don't drop the last buffer of data they
supplied.

The device ID is invalid as soon as the device is closed, and is eligible
for reuse in a new [SDL_OpenAudioDevice](SDL_OpenAudioDevice)() call
immediately.

## Version

This function is available since SDL 3.0.0.

## Code Examples

```c++
extern SDL_AudioSpec want;
SDL_AudioDeviceID devid = SDL_OpenAudioDevice(NULL, 0, &want, NULL, 0);
if (devid > 0) {
    SDL_PauseAudioDevice(devid, 0);
    SDL_Delay(5000);  // let audio callback run for 5 seconds.
    SDL_CloseAudioDevice(devid);
}
```

## Related Functions

* [SDL_OpenAudioDevice](SDL_OpenAudioDevice)

----
[CategoryAPI](CategoryAPI), [CategoryAudio](CategoryAudio)

