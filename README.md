# MPDN  
_Music Player Daemon Notifications_  

---  

__Dependencies:__  
    - `dunst`  
    - `dunstify` _# Some distributions of dunst do not include dunstify_  
    - `ffmpeg`  
    - `mpc`  
    - `mpd`  

__Install:__  
1. Clone this repository to `$XDG_CONFIG_HOME/mpdn` or `$HOME/.config/mpdn`  
2. Link the executable to `$PATH`:  
    - `ln -si $XDG_CONFIG_HOME/mpdn/bin/mpdn $HOME/.local/bin/mpdn`  
  __OR__  
    - `ln -si $XDG_CONFIG_HOME/mpdn/bin/mpdn /usr/bin/mpdn`  

__Hooking into Hyprland:__  
`bind = $mainMod, SPACE, exec, mpdn -P` _# MOD + Space Pauses/Plays mpd and displays status_  
`bind = $mainMod, M, exec, mpdn -k` _# MOD + M Displays playback status with no changes_  
`bind = $mainMod, N, exec, mpdn -n` _# MOD + N Go to next song and display status_  
`bind = $mainMod, P, exec, mpdn -p` _# MOD + P Go to previous song and display status_  
