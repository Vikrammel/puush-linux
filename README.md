Puush in Linux
=====================

Takes screenshots and uploads them to puush using the puush API and copies the link to clipboard. Recommended for set up with keyboard shortcuts
<br>Utilises __shutter__ for taking screenshots, __zenity__ for file uploads (shutter not included in X/L/Ubuntu).

## Instructions
- Clone or download the repo
- In file "puush" add your puush API key to PUUSH_API_KEY
  - (You can find your API key at http://puush.me/account/settings)
- Make it executable using __chmod +x puush__
- Place this file wherever you want (recommended: /usr/local/bin)
- Install shutter if not present (check with `shutter -v`) using `sudo apt-get install shutter`
- Set up keyboard shortcuts within linux
  - (in Ubuntu it's system settings > keyboard > keyboard shortcuts > custom shortcuts)
  - (in Xubuntu it's keyboard > application shortcuts > add)
  - Log out for the changes to take place
  - Here's what it looks like for mine: ![Puush keyboard setup](http://puu.sh/cOyVz/8dcb1cd498.png)

### Commands
``` bash
puush -d		# puush desktop
puush -r		# area puush
puush -w		# puush current active window
puush -f		# file upload

puush -h  	  # help
```

## Dependencies
- shutter
- zenity
- curl
- xclip
- notify-send


### Alternatives
- puush in command line https://github.com/blha303/puush-linux
- puush using keyboard https://github.com/sgoo/puush-linux

originally made by Sunmock Yang, modified by Vikram Melkote
