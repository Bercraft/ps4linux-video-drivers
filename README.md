# ps4-video-drivers

Video drivers required to use 3d hardware acceleration on Arch Linux.
Original patches from failoverflow: https://github.com/fail0verflow/ps4-radeon-patches

Patch for ps4pro (GLADIUS) from eeply.

We just set up a repository where you can get pre-patched video drivers for ps4

1) Add the repository to /etc/pacman.conf
```
sudo echo -e "\n[ps4]\nSigLevel = Never\nServer = https://psxita.it/repo-testing" >> /etc/pacman.conf
```

2) Update Arch Linux
```
sudo pacman -Syu
```

3) Install the drivers
```
sudo pacman -S mesa-git lib32-libdrm-git lib32-mesa-git libdrm-git xf86-video-amdgpu-git
```

4) Reboot Arch Linux

The drivers will be periodically updated and installed automatically when you upgrade Arch Linux


NOTE:
If you for some reason need the old drivers you can still get them from this repository:
```
https://psxita.it/repo
```
