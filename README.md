# music_plugin
Music plugin for polybar which enables toggling between displaying "artist - title" and "album".


This is a modified version of mpris.sh, a plugin provided in polybar's User Contributed Modules page. It contains a function that enables clicking on the module in polybar to toggle between displaying "artist - song title" and "album".

To add this plugin to polybar, place the script provided in the same folder as polybar's config file, and add the following module to the polybar config:

```
[module/music]
type = custom/script
interval = 1

label = %output:0:40:...%
exec = ~/.config/polybar/music.sh
click-left = ~/.config/polybar/music.sh --click
```
