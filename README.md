# Linux
Tips for Linux (PopOS!) and Awesome WM

# Use Nala instead of apt
sudo apt install nala
[Nala repo and info](https://gitlab.com/volian/nala)

# Gnome Tweaks
Needed for icon packs, theming and text configuration, etc..
sudo nala install gnome-tweaks

# Awesome WM
## Enable Natural (reverse) Scrolling on Trackpad

- Find the ID of your trackpad by running the ``xinput`` command. In my case it was 18.
- View the properties of your trackpad by running:
``xinput list-props 18`` substituting your ID with mine]

- You'll likely see this, or a similar, line near the top of the lengthy output. ```libinput Natural Scrolling Enabled (313):     0``` Note that your output may show a different number than 313. The important part is the zero, meaning 'false' for natural scolling. This is the problem. Next is the solution.

- Type ``xinput set-props "PS/2 Generic Mouse" "libinput Natural Scrolling Enabled" 1`` to set the natural scrolling property to 'true'. Substitute the device name of your trackpad in quotes as returned by the `xinput` command previously run. Done!

# Nord Theme and Icons

[Blue Zafiro Plus icon pack](https://www.pling.com/p/1412411)

[Nord Dark Blueish Accent theme](https://www.pling.com/p/1267246/)
