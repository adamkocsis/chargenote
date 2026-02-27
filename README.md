# Charging notification 

Notify users that a charging battery has reached a given percentage (default 80%). 

This small application was developed because I got fed up that I could not find an application that would alert me when I am charging my old tablet that it's battery would be overloaded.


## Requirements

- acpi: used to get the battery state.
- vlc: used to play the alarm.
- alsa mixer-amixer (optional): used to unmute the speakers so the alarm is running.


## Installation


1. Clone repository:
`git clone ...`

2. Move directory to whereever you want

3. Use `nohup`

``` sh
nohup ./charenote
```





