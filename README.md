#Keyboard Spectrograph for Corsair RGB series keyboards and mice.

#Note
Please note that this is **not** the similar, but far more advanced Corsair Effects Engine. This code is pretty much archaic at this point, and is only here for reference.

#Summary
This application is made to run in the place of the Corsair Utility Engine. It provides several effects that are not available through CUE, such as a spectrograph for audio playing through the computer or from input devices, randomized lighting, reactive lighting effects, idle/away timer with profile switching, and other features. It is still in active development, and there are many new features on the way!

Build
-----

To build the software, you need to get the device profiles. They aren't present
in the repository, although they're available as part of the 0.6.4a installer on
the archived version of Emily Maxwell's website. so you'll need to download them
from the [web archive][device-profiles], and unpack `corsair_devices` directory
from the downloaded archive into
`Corsair RGB Keyboard Spectrograph/corsair_devices`.

#Installation
Please ensure that you are running .NET 4.5+. You can download it <a href="http://www.microsoft.com/en-ca/download/details.aspx?id=30653">here</a>.
Download the compiled binaries from <a href="http://emily-maxwell.com/?page=keyboardspectro">my website</a>, and extract them to a location of your choice.

#Usage
When you launch the program for the first time, it will open up to the Settings tab. Here, you should select the keyboard model that you're using, and then which layout you're using. To the right of this, you can select which mouse you're using as well, and have the effects extend to it. (Note that Spectro doesn't extend to the mouse yet, only the stuff on the Effects tab)

With your keyboard and mouse selected, click on the Spectro tab. Select what you want your foreground and background colours to be (foreground is on top, background is on the bottom), and then choose your audio source. If you select Output, it'll capture whatever is being played through your system's default output device. Select input to use a microphone, line-in, or other input device for capture instead.

Hit Start, and play some music!

If you find that it's not picking up your audio very well, try turning up the sensitivity. If you want to slow down or speed up the effects, change the Refresh Delay (my personal favourite is a value of 10).

#Upcoming Features
Reactive Typing
Heatmap
Mouse heat lighting
STRAFE support
Windows audio device mute state observation (to toggle the mute button's colour)
Rework of rendering engine

#Known Issues
- AMD HDMI Audio drivers don't play nicely with, well, anything. It's possible that you'll have issues if that's your default output device.
- Spectro background effects can stop when there is no audio stream. This is due to WASAPI closing the stream. This will be corrected with the engine rework.

#More Info
Check out the main forum thread at http://forum.corsair.com/v3/showthread.php?t=139027
Changelog and other information: http://emily-maxwell.com/

#License
This project is licensed under the GNU GPL v3.0. When using snippets of my code, please ensure the following or something similar prefaces it:

Written by Emily Maxwell. https://github.com/Elestriel/Corsair-RGB-Keyboard-Spectrograph

## ColorPickerControls

This project includes code portions from [WPF Color Picker Contruction
Kit][color-picker] ditributed under the terms of [The Code Project Open License
(CPOL)][cpol]. All that code is stored in the [ColorPicker][colorpicker-src] directory.

#Cheers!
I hope you enjoy using this program as much as I enjoy making it!

[colorpicker-src]: ColorPicker/

[cpol]: https://www.codeproject.com/info/cpol10.aspx
[color-picker]: https://www.codeproject.com/Articles/131708/WPF-Color-Picker-Construction-Kit
[web-archive]: https://web.archive.org/web/20151012073044/http://emily-maxwell.com/?page=keyboardspectro
