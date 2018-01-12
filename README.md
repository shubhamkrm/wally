# wally
It is a command line utility to download a random wallpaper from the internet and set it as the desktop background.

## Dependencies
Wally requires the following tools to be installed:
1. `feh`: It is used to set the wallpaper
2. `curl`: It is used to make HTTP requests
3. `jq`: It is used for parsing json

These utilities are generally available in the default distro-repositories

Wally can be used to change the wallpaper at fixed intervals, and this can be achieved using a `cron` job.
To create a cron job, type
    
    $ crontab -e
    
This will open crontab file with your default editor. In this file, add:

    @hourly /path/to/wally
