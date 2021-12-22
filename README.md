# headsetcontrol for py3status
**using (external_script) module**

i made this for my corsair hs70 but it may work for other supported headsets that headsetcontrol uses

*__Requirements:__*

 - [headsetcontrol](https://github.com/Sapd/HeadsetControl) this is available for arch users via AUR
 - py3status


my i3status.conf settings for the script

```
order += "external_script hs70"

external_script hs70 {
    format = "[<span color='#000' bgcolor='#E9E600' size='large'>  </span><span color='#E9E600'>{output}</span>]|<span color='#000' bgcolor='#222' size='large'>  </span><span color='#F00'></span>"
    script_path = "~/.config/i3/scripts/hs70.sh"
    interval = 5
    separator = false
}
```

if you want to hide the module when you aren't connected edit your config and remove the text after the pipe |
```
format = "[<span color='#000' bgcolor='#E9E600' size='large'>  </span><span color='#E9E600'>{output}</span>]|"
```
