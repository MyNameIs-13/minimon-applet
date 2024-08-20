# Minimon COSMIC Applet

A little applet for displaying total CPU load and/or memory usage. Can sit in the panel or Dock. Can display as icons or text.  

![Dock](https://github.com/user-attachments/assets/a0314649-3ffd-49a6-88cb-ae655a293977)

![panel-circles](https://github.com/user-attachments/assets/5ad4fa80-d461-4cd3-aa92-ea25a09339d3)
![screenshot-2024-08-15-00-50-20](https://github.com/user-attachments/assets/4a99da4b-326d-4462-8430-154335390096)

![screenshot-2024-08-15-01-02-19](https://github.com/user-attachments/assets/c1e8bc40-d678-44d0-ae6e-e3036102f4a1)

![color-picker](https://github.com/user-attachments/assets/9a40ce00-cf8e-4c03-ae1d-602e4904a601)


Thanks to [@edfloreshz](https://github.com/edfloreshz) for the applet template :)

## Installing
If you're on a .deb based distibution download [latest version](https://github.com/Hyperchaotic/minimon-applet/releases) and install with the following commands:

```sh
unzip ./cosmic-applet-minimon_0.1.1_amd64.deb.zip
dpkg -i cosmic-applet-minimon_0.1.1_amd64.deb
```

## Building

To build your COSMIC applet, you will need [just](https://github.com/casey/just) and probably xkbcommon, if you're on Pop!\_OS, you can install it with the following command:

```sh
sudo apt install just libxkbcommon-dev
```

After you install it, you can run the following commands to build and install your applet:

```sh
just build-release
sudo just install
```

Alternatively generate a deb file for installation:

```sh
just deb
```
and install with:

```sh
sudo dpkg -i <name_of.deb>
```

