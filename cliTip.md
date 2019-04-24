### Tips and Useful Links for CommandLIne

#### Gnome setting from other Desktop Environment
- with command `env XDG_CURRENT_DESKTOP=GNOME gnome-control-center`

#### ls command
- [displaying only directories](https://stackoverflow.com/questions/14352290/listing-only-directories-using-ls-in-bash-an-examination)
	* `ls -d */`
	* */ matches every directories, -d only displays subdir, not it's contents
- ignore certain files: `ls -I`
	- [ignore certain file in ls](https://askubuntu.com/questions/512961/exclude-certain-files-in-ls)
#### file comparison cmd
- [How to Compare Two Files in Unix: File Comparison Commands](https://www.softwaretestinghelp.com/compare-two-files-unix/)
	- `diff -q dir1 dir2`
##### bashrc tips
- [bash aliases](http://stefaanlippens.net/my_bashrc_aliases_profile_and_other_stuff/)

#### Opening files
- [How to open file when I don't know the command for it?](https://askubuntu.com/questions/236631/how-can-i-open-a-file-when-i-do-not-know-what-command-opens-it)
- use `gnome-open filename`, to use default gnome program

##### apt and apt-get difference
- [Difference Between apt and apt-get Explained](https://itsfoss.com/apt-vs-apt-get-difference/)
##### Bluetooth

- Turn bluetooth on/off from cli
[bluetooth on off from cli](https://askubuntu.com/questions/380096/turn-on-off-bluetooth-from-shell-not-from-applet)
##### wireless 
- start / restart network manager
[How to restart the networking service?](https://askubuntu.com/questions/230698/how-to-restart-the-networking-service)
##### Termianl tab
- terminal tabs showing command running
[Ask ubuntu: Make gnome-terminal show the command running as title](https://askubuntu.com/questions/126737/make-gnome-terminal-show-the-command-running-as-title)
##### Vim
- vim system clipboard copy and paste
[How can I copy text to the system clipboard from vim?](https://vi.stackexchange.com/questions/84/how-can-i-copy-text-to-the-system-clipboard-from-vim)
	- make sure to check the .vimrc entry
- vim colorsheme not working
	- bring `call pathogen#infect()` all the way top of the .vimrc
	- [E185: cannot find color scheme..](https://stackoverflow.com/questions/8804767/e185-cannot-find-color-scheme-solarized)

##### Zip/Unzip
- Tar -... command
- [How-To Geek-howtoUsingTar](https://www.howtogeek.com/248780/how-to-compress-and-extract-files-using-the-tar-command-on-linux/)

##### Debian Package
- \~~~.deb file
- [What is a Debian Package??](https://www.debian.org/doc/manuals/debian-faq/ch-pkg_basics.en.html)
- install .deb package with...
	* `sudo dpkg -i /path/to/deb/file` followed bt... `sudo apt-get install -f`  or...
	* `sudo apt install /path/to/package/name.deb`

##### [Htop system](Htop-system) monitor
- [__Youtube-How_to_use_htop__](https://www.youtube.com/watch?v=Qw2ZUf0hTF8)

#### Customizing gnome as Mac OS
- [Make Gnome 3 look like mac OS X in ubuntu 17.04, 16.10](http://ubuntuhandbook.org/index.php/2017/05/make-gnome-3-look-like-mac-os-x-in-ubuntu-17-04-16-10/)
- [set custom fonts on ubuntu, ubuntu-wiki](https://wiki.ubuntu.com/Fonts)
- [Yosemite-shell theme](https://www.gnome-look.org/content/show.php/Yosemite+Shell?content=166200)
#### Macbuntu 17.04 pack
- [Mac Buntu pack](http://www.noobslab.com/2017/06/macbuntu-transformation-pack-ready-for.html)

#### Github
- [How to list all tracked file](https://stackoverflow.com/questions/15606955/how-can-i-make-git-show-a-list-of-the-files-that-are-being-tracked)
- [removing a file from Git repo without deleting it locally](https://stackoverflow.com/questions/1143796/remove-a-file-from-a-git-repository-without-deleting-it-from-the-local-filesyste)
	- git ls-tree -r master --name-only
- [Git trying to push untracked files](https://stackoverflow.com/questions/44285232/git-counting-too-many-files-and-tries-to-push-untracked-files)
	- `git rebase -i origin/master`   command to edit the commit history

#### App menu and icons
- [desktop file configuration](https://askubuntu.com/questions/410053/how-do-i-install-3rd-party-programs-and-make-them-appear-in-the-dash-home-menu)
#### Ipython notebook
- [convert ipynb into other format](https://stackoverflow.com/questions/18140964/return-different-type-of-data-from-a-method-in-java)
		- `ipython nbconvert "notebook.ipynb" --to html`
#### Hardware Deteils
- [hardware details on cli](https://askubuntu.com/questions/31618/how-can-i-find-my-hardware-details)
- [computer_model](https://askubuntu.com/questions/386927/how-to-know-the-model-of-the-computer-from-ubuntu)
#### Touchpad setting
- [xinput setting](https://wiki.archlinux.org/index.php/Libinput)
- [xinput_setting_basic](https://faq.i3wm.org/question/3862/system-settings-not-working-scrolling-and-touch-click.1.html)
### if can't mout as readwrite, 
- unmount everything and kill the process, by fuse, and mount it again

### Log out via terminal
- `gnome-session-quit`
### python gi module error
- [How to install gi module for anaconda python3?](https://stackoverflow.com/questions/37526026/how-to-install-gi-module-for-anaconda-python3)
## Ipthon Tips
### Execute / import packages on startups
- [Automatically import modules when entering ipython](https://stackoverflow.com/questions/11124578/automatically-import-modules-when-entering-the-python-or-ipython-interpreter)
#### bash aliases, providing arguments ####
[complex bash aliases with arguments](https://stackoverflow.com/questions/4060880/passing-argument-to-alias-in-bash)

### Cat command, piping input from ls
[piping input from ls to cat](https://stackoverflow.com/questions/26443951/why-not-pipe-list-of-file-names-into-cat)
### Bash Scripting Tutorial
[Shell Scripting TUtorial](https://www.shellscript.sh/)

### Disable touchpad while typing
- [disable touchpad while typing](https://askubuntu.com/questions/886092/how-do-i-disable-the-touchpad-while-typing)
- [editing xorg...libinput config](https://askubuntu.com/questions/649103/proper-touchpad-thumb-palm-detection-with-libinput#678122)

### Synclient
- synclient set up config for touchpad, under /usr/share/X11/xorgconfig.d/70-synaptics.conf
	- `Option "option_name" "int"`
- e.g. to enable horizontal natural scrolling:
	- `synclient HorizScrollDelta=-113` negative for natural scrolling
- [synclient](https://wiki.archlinux.org/index.php/Touchpad_Synaptics)
- [palm detection](http://add4jhf.blogspot.com/2013/09/touch-pad-deactivation-while-typing-and.html)
- set synclient VertEdgeScroll = 0

### App Image files
- don't require installation, just start using it
- [how to use AppImage on Linux](https://itsfoss.com/use-appimage-linux/)

### Extending Partintion to the left with live USB
- [Gparted: Move extended partition to the left](https://askubuntu.com/questions/557751/gparted-move-extended-partition-on-the-left)
### Disable touchpad while typing
- [disable using syndaemon](https://wiki.archlinux.org/index.php/Touchpad_Synaptics#Disable_touchpad_while_typing)
- `syndaemon -i 0.5 -t -k &`

### see file system usage
- `df` command, to see which file system's size

### Creating Live USB with dd command
- [live ubuntu usb](https://www.cyberciti.biz/faq/creating-a-bootable-ubuntu-usb-stick-on-a-debian-linux/)
- [live Kali usb](https://docs.kali.org/downloading/kali-linux-live-usb-install)
-

### Unzip file on another directory
- [unzip to another directory](https://askubuntu.com/questions/45349/how-to-extract-files-to-another-directory-using-tar-command)

### apt package search command
- `apt search <keyword>`

### Resizing image file size in terminal
- `jpegoptim --size=desired_sizek /path/to/image.jpg`
- [How can I change a picture's file size?](https://askubuntu.com/questions/818593/how-can-i-change-a-pictures-file-size)
