## Ubuntu Tips

1. PGP with evolution email
	- [Pretty Good Privacy with evolution](https://www.linux.com/learn/how-enable-pgp-encryption-evolution)
2. Using HDD as RAM, by swap space
	- [How to use hard disk as RAM like windows](https://askubuntu.com/questions/349156/how-to-use-hard-disk-as-ram-like-in-windows)
4. Command line tips
	- [cliTip](cliTip)
5. FIrefox Quantum TouchScreen
	- [askubuntu](https://askubuntu.com/questions/978226/how-to-make-touch-screen-scrolling-work-in-firefox-quantum)
6. Facebook messenger for Linux
7. 	- [how to install FB messenger Linux Client](https://tomsondev.bestsolution.at/2014/11/05/efxclipse-1-1-new-features-generate-controller-from-fxml/)
8. window buttons to left/right
	- [move windows buttons to left](http://tipsonubuntu.com/2017/10/10/ubuntu-17-10-tip-move-window-buttons-min-max-close-left/)
9. window manager tile
	- [i3 for ubuntu 17](https://www.reddit.com/r/i3wm/comments/5x13z3/willdoes_i3_work_on_ubuntu_1704/)
10. fix 'all squared' icon tray on PIA on ubuntu 17.10
	- [PIA fix for Ubuntu 17.10](https://www.privateinternetaccess.com/forum/discussion/27543/ubuntu-mate-17-10-with-pia-v74)
11. fixing wifi connected but no internet
	- [Ubuntu 17.04 connected to wifi but can't browse internet](https://askubuntu.com/questions/907763/ubuntu-17-04-connected-to-wifi-but-cant-browse-internet)
	- Disable DNSSEC:
		- `sudo mkdir -p /etc/systemd/resolved.conf.d`
		- `printf "[Resolve]\nDNSSEC=no\n" | sudo tee /etc/systemd/resolved.conf.d/no-dnssec.conf`

	- Reconfig resolvconf:
		- `sudo dpkg-reconfigure resolvconf`
		- `# Say yes to "prepare /etc/resolve.conf for dynamic updates?"`
