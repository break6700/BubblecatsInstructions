# How to install Ubuntu on a Chromebook
To get to Developer Mode, we need to first reboot into Recovery Mode. On most Chromebooks, you do so by turning the device off, then holding down the `ESC` and `Refresh` keys while you press the Power button.

Once in this mode, press `Ctrl-D`. You will be prompted with an opportunity to “turn OS verification OFF”. Press `Enter` to do so.

When you boot up your Chromebook, it will begin with a warning screen noting that “OS verification is OFF”. You will need to press `Ctrl-D` to continue. Your device will now transition to Developer Mode. **THIS WILL WIPE YOUR MACHINE**

Every boot thereafter will also begin with that warning screen, and a need to press `Ctrl-D` to continue. Do not follow the onscreen instructions to turn OS verification on, or you risk wiping your machine’s data and turning Developer Mode off. 

1. Go to [https://goo.gl/fd3zc](https://goo.gl/fd3zc), this will download the laterst version of crouton.
2. `CTR-ALT-D` will open a terminal window in your browser. Type "shell" then enter.
3. Copy the installer to an executable location by running `sudo install -Dt /usr/local/bin -m 755 ~/Downloads/crouton`
4. Now that it's executable, run the installer itself: `sudo crouton -t unity
5. Wait patiently and answer the prompts like a good Ray of sunshine.
6. Done! You can jump straight to your Ubunutu session by running `sudo startunity`
7. Cycle through Chromium OS and your running graphical chroots using `Ctrl+Alt+Shift+Back` and `Ctrl+Alt+Shift+Forward`.
8. Exit the ubuntu by logging out of Unity.

If you run into an issue with SD card/external storage compatibilty:
- Ensure that the drive is plugged in **before** you boot into Ubuntu
- Make sure it is in an appropriate format (may run into issues with exFAT)
- If it doesn't show up, open `Disks` and choose the drive, cick the directory link and create a shortcut to that directory and save in the bookmarks in the file explorer.
