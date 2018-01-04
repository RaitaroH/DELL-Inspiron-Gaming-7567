# Model
DELL 15.6'' Inspiron Gaming 7567, 1080p 60Hz IPS, Procesor Intel® CoreTM i7-7700HQ (6M Cache,up to 3.80 GHz), 8GB DDR4, 1TB + 8GB SSH, GeForce GTX 1050 Ti 4GB, Linux, Black

I also added: SSD ADATA SX8000 128GB PCI Express 3.0 x4 M.2 2280. Now, I did not know this laptop DOES NOT support NVMe but fuck it.

# My experience
This is going to be my experience with the DELL Gaming 15.6'' Inspiron 7567. I did find reviews of this laptop BUT on the Windows side.

The laptop runs really well, crushing pretty much anything. The packaging was not branded too much so don’t worry about that. I also got a red backpack for the laptop. I have to say it holds the laptop really well.

The screen is 1080p 60Hz and it is NOT A TN panel. I was worried I would get the TN panel, but no. This screen looks really nice.
An interesting thing is the hinge. The laptop can be opened one handed, BUT you can also keep it one hand, holding it from the back without having it fall (I don't promise you won't drop it). Is not a thinkpad or something but it does work. Nice surprise. Keep in mind that the laptop is quite heavy so maybe not the best option.

The speakers are quite loud, though very directional. I almost never go above 50% unless the audio for something is quite low. At 100% or 150% (enabled that) the audio gets distorted as you would expect.

The keyboard is only in red backlight, 3 steps (none, 50%, 100%). Not bad but I don’t love it or something like that. If you hit some keys besides dead on they kinda feel like they missed the mark.

The touchpad is good. No separate buttons but it is good. In KDE I don't see any fancy options for it like zoom and alike. I can put one finger down and use another to scroll, not just do that on the right side. I did not activate any corner stuff either.

The ports are quite nice on this. I did use the ethernet so I didn’t have to set the wifi, but the wifi can easily reach 10Mb/s + on my network so…

The battery isn’t the best in the world but what would you expect for a gaming laptop. The laptop charges quite fast and the cable has a blue light (I actually like it because it is enough light to see around in the dark after I closed my laptop). The brick also has a nice strap to keep stuff nice. The charger also was compatible with Europe so I didn't have to do anything.

# Temperature and Unigine Heaven benchmark
The temperatures are quite… I could even say bad, maybe. The fan is quite loud but it only kicks in after 60+ degrees (you cna change that with software).
The CPU gets kinda toasty (50-60°C at idle; 70-80°C during heavy load like gaming; I did rectify that bellow) the GPU is much better (45-50°C at idle; doesn’t pass 65 during heavy load), the cooling can keep it under control (for more temperature info look below). Now, I would like to ask the people in here if they thing this is dangerous. I did find that the max temperature allowed  is 100°C for the CPU and around 75/95°C for the GPU. That is fine but still…
I also red these:
https://www.reddit.com/r/intel/comments/6fs2vw/i7_7700hq_operating_temps_question/
also this:
https://www.reddit.com/r/intel/comments/6qsmmn/intel_i7_7700hq_temps_way_too_high/


So I did go in the BIOS and disabled TurboBoost and this reduced the max CPU temp to 70°C (max 72) from 80 or so. Also the GPU ended up around 60-65°C (sometimes 66). No deep in fps or overall performance. Keep in mind that I even wrote this line ( in libre writer) as the Unigine Heaven benchmark was going. Here is the result in basic and in extreme:

![alt-tag](https://raw.githubusercontent.com/RaitaroH/DELL-Inspiron-Gaming-7567/master/Images/Heaven1a.png)
![alt-tag](https://raw.githubusercontent.com/RaitaroH/DELL-Inspiron-Gaming-7567/master/Images/Heaven1b.png)

I also went in the BIOS and disabled HyperThreading. In short it was worse on temperatures (under heavier load; almost the same on idle) but slightly better on performance under heavy load according to the benchmark. The slight differences are most likely insignificant. In my opinion I would rather not do this.
Here are the results:
The CPU temp was around 74°C reaching even 76°C. The GPU was around 68-70°C. So much worse than before. 
I also redone the Unigine Heaven test in extreme mode and here is the result:

![alt-tag](https://raw.githubusercontent.com/RaitaroH/DELL-Inspiron-Gaming-7567/master/Images/Heaven2.png)

OTHER BIOS changes:
I did go in the BIOS and played around with a few things: activated virtualization, made sure secure boot and alike are disabled. I also changed boot order for Linux installation in order to install the OS. I also changed the FN keys to work as F1...F12 first and be modified with Fn instead of the inverted default. I also went ahead and made the keyboard not be lit all the time under AC Power. I also disabled the webcam and mike.

# Gaming
Well see above for fps. I also installed VMware. The youtuber `egee` made some videos about it so you can look at those. Nothing fany like Nier;Automata would work there so you know. It works well for very light games (say VNs) and older games.

For emulation though you can try [rpcs3](https://rpcs3.net/). I did try it out with Persona 5 and it worked rather well. The CPU does get toasty as above though but the game is playable. Some sound problems at first but during the game it was fine. I did not try it out with the BIOS changes mentioned above. I will update this after I try it out.
UPDATE: The temperature went from 80 to 65 while using the emulator to play Persona 5. That is quite the improvement. The game also runs like it did before.

# Linux and inxi -F
When it comes to linux I put KDE Neon 5.11 on here and it runs just beautifully. To be fair I tried to install Antergos but it hanged at boot from the USB, just so you know. I decided that hey, if I don’t want to bother fixing antergos not booting I don’t think I would like to bother fixing other problems that may arise.


Now more info about the system with linux on:
```
Kernel:    4.10.0-42-generic x86_64 (64 bit) Desktop: KDE Plasma 5.11.5
           Distro: neon 16.04 xenial
Machine:   System: Dell (portable) product: Inspiron 15 7000 Gaming
           Mobo: Dell model: 065C71 v: A00 Bios: Dell v: 01.00.06 date: 04/26/2017
CPU:       Quad core Intel Core i7-7700HQ (-HT-MCP-) cache: 6144 KB 
           clock speeds: max: 3800 MHz 1: 2379 MHz 2: 2039 MHz 3: 1118 MHz 4: 2308 MHz 5: 2480 MHz 6: 1003 MHz
           7: 2647 MHz 8: 1398 MHz
Graphics:  Card-1: Intel Device 591b
           Card-2: NVIDIA Device 1c8c
           Display Server: X.Org 1.19.5 driver: nvidia Resolution: 1920x1080@60.02hz
           GLX Renderer: GeForce GTX 1050 Ti/PCIe/SSE2 GLX Version: 4.6.0 NVIDIA 387.34
Audio:     Card Intel Device a171 driver: snd_hda_intel Sound: ALSA v: k4.10.0-42-generic
Network:   Card-1: Realtek RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller driver: r8169
           IF: enp2s0 state: down mac: 50:9a:4c:bf:86:9c
           Card-2: Intel Wireless 3165 driver: iwlwifi
           IF: wlp3s0 state: up mac: ac:ed:5c:d0:93:00
Drives:    HDD Total Size: 1000.2GB (28.4% used) ID-1: /dev/nvme0n1 model: N/A size: 128.0GB
           ID-2: /dev/sda model: ST1000LX015 size: 1000.2GB
Partition: ID-1: / size: 23G used: 8.4G (39%) fs: ext4 dev: /dev/nvme0n1p1
           ID-2: /home size: 95G used: 23G (26%) fs: ext4 dev: /dev/nvme0n1p5
           ID-3: swap-1 size: 5.00GB used: 0.00GB (0%) fs: swap dev: /dev/sda1
RAID:      No RAID devices: /proc/mdstat, md_mod kernel module present
Sensors:   System Temperatures: cpu: 59.0C mobo: N/A gpu: 50C
           Fan Speeds (in rpm): cpu: N/A                                                                                                                                  
Info:      Processes: 251 Uptime: 29 min Memory: 2132.8/7626.4MB Client: Shell (bash) inxi: 2.2.35

```

# Nvidia drivers
Everything I will say from now applies to KDE Neon 5.11: It installed without problems

NVIDIA:
```
sudo apt-add-repository ppa:graphics-drivers/ppa -y
```
And I installed nvidia-387 after this. The latest at the time of this writing.

# Locale
Languages:
It has some issues with the locales, but I think is KDE specific. To fix that I added to .bashrc this:
```
# locale
export LC_ALL=en_US.UTF-8
export LANG=en_US.UTF-8
export LANGUAGE=en_US.UTF-8
```

Regarding japanese input, if somebody is interested I used ibus. fcitx doesn’t work well with Qt from I noticed.
```
# Japanese input
sudo apt-get install -y ibus ibus-qt4 ibus-anthy ibus-gtk ibus-gtk3
```
And for it to work properly add this to .bashrc:
```
export GTK_IM_MODULE=ibus
export XMODIFIERS=@im=ibus
export QT_IM_MODULE=ibus
ibus-daemon -drx
```
I would also recommend to use anthy all the time and use a keyboard shortcut to switch it off instead of going to another input. For some reason changing input from anthy to en takes a lot more key presses for some weird reason.

Also I have the romanian keyboard set to a keyboard shortcut. Everything is fine BUT I would recommend not to install additional languages. For me certain applications take the language. For example VLC goes to romanian and audacious goes to japanese for some weird reason. So I rather not. 
Regarding japanese names in the terminal… they do display and I can even use tab for autocompletion. So that is rather nice.

# Applications
Extra packages you might want:
```
# Installing more stuff
sudo apt-get install -y synaptic ffmpeg libreoffice libreoffice-l10n-en-gb ubuntu-drivers-common ubuntu-restricted-extras keepassx gufw brightside imagemagick htop gimp gnome-disk-utility  libnotify-bin

# QT stuff
sudo apt-get install -y qalculate yakuake kdesudo filelight ktorrent inkscape krename

# Redshift
sudo apt-get install -y redshift geoclue-2.0 geoclue-hostip

# Kde thumbnails for dolphin
sudo apt-get install -y kdegraphics-thumbnailers ffmpegthumbs -y

# Removing flash from the system
sudo apt-get remove adobe-flashplugin flashplugin-installer -y

# Git stuff
sudo apt-get install -y git

# youtube dl
sudo wget https://yt-dl.org/downloads/latest/youtube-dl -O /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl
```

Now, you can use gnome-disk-utility for disk checking and USB iso writing. I think is useful.
kdesudo is to open kde applications as root.
I also went ahead and installed synaptic too. See down bellow how to make it look good under root.


To use the breeze-dark theme in root apps (or you know, make it look good)
```
# Dark theme as root
sudo bash -c "echo 'XDG_CURRENT_DESKTOP=\"KDE\"' >> /etc/environment"
kdesudo systemsettings5
```
Change the theme in the systemsettings5.


As a music player I installed audacious because I like it. Go for the ppa to use the Qt version.
```
sudo add-apt-repository ppa:nilarimogard/webupd8 -y
sudo apt-get update
sudo apt-get install conky-manager -y
```
Use `audacious --qt` to open it as qt.


For conky:
```
sudo add-apt-repository ppa:teejee2008/ppa -y
sudo apt-get update
sudo apt-get install conky-manager -y
```
Also my repo here, if you are interested.
https://github.com/RaitaroH/Conky-Breeze


Also if you are interested in Yakuake, I could not install any themes so I cloned breeze dark perfect. Here is the code you can use. Just put it in a script or go to the git clone directly:
```
if [ -d ~/.local/share/yakuake/kns_skins ]; then
	echo "Yakuake theme folder exists. Skipping."
else
	mkdir ~/.local/share/yakuake/kns_skins
	git clone https://github.com/noahadvs/yakuake-breeze_perfect_dark.git  ~/.local/share/yakuake/kns_skins/
fi
```


You may also want to use KDE Connect:
```
# Enable firewall
sudo ufw enable
# KDE Connect:
sudo ufw allow 1714:1764/udp
sudo ufw allow 1714:1764/tcp
sudo ufw reload
```


GRUB changes; skip grub and auto boot in linux
```
GRUB_CMDLINE_LINUX_DEFAULT=""
GRUB_HIDDEN_TIMEOUT=0
GRUB_HIDDEN_TIMEOUT_QUIET=true
GRUB_TIMEOUT=10
```


Webcam disable. I know I did in the BIOS too, but just to be safe.
```
# Disable webcam
sudo bash -c "echo 'blacklist uvcvideo' >> /etc/modprobe.d/blacklist.conf"
```

# Extra stuff
If you are interested in libreoffice breeze-dark theme check my repo here:
https://github.com/RaitaroH/LibreOffice-BreezeDark

If you are interested in changing wallpapers in KDE check my repo:
https://github.com/RaitaroH/KDE-Terminal-Wallpaper-Changer

Also if you are interested in dark themes with the breeze dark colors check, yet again, my stuff:
https://github.com/RaitaroH/Import-All-Deepdark
