# Charging notification 

Notify users that a charging battery has reached a given percentage (default 80%). 

This small application was developed because I got fed up that I could not find an application that would alert me when I am charging my old tablet that it's battery would be overloaded.

## Requirements

- acpi: used to get the battery state.
- vlc: used to play the alarm.
- alsa mixer-amixer (optional): used to unmute the speakers so the alarm is running.


## Installation and running


1. Clone repository:
`git clone https://github.com/adamkocsis/chargenote`

2. Move directory to whereever you want. Use cd to enter the directory. Change the script to an executable with

``` sh
chmod +x ./chargenote
```

3. Single run (optional): use `nohup` to suppress the SIGHUP and put the process in the background. Change the `chargenote` variable to whereever the `chargenote` executable is located.

``` sh
chargenote="/mnt/sky/Dropbox/System/GNU/chargenote/chargenote"
nohup $chargenote &
```

You can kill the process by finding its process ID (PID) and then killing it:

``` sh
kill <PID>
```

4. Persistent run: Add the line above at 3. to `~/profile` which will run the process at login.  

## Configuration

You can put the alarm sounds in the `alarms` directory, and modify the `chargenote` file. 


