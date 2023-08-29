# hyprland_conf
Current configuration for Hyprland Arch Linux

# Animation not smooth problem:
No `swaybg`, if wallpaper is needed, I would sugguest yay others like `hyprpaper`
Maybe bullshit like battery contrl

# flickering problem on AMD
Please rendering using your `Integrated Graphics` (if not Nvidia) if you have 2 GPU running on. See "Switching Multi GPU" section on Hyprland Wiki
If you have `seatd` error like could not connect or could not find, try following:
```
systemctl enable seatd
systemctl start seatd
sudo usermod -a -G seat myusername
```
This should solve the error and may solve the flickering problem
