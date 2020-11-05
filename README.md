![Fuxion logo](https://github.com/anonymousproo/Fix-W-Target-Packages-is-configured-multiple/blob/main/jbk0qhan1gh7.png)

![Fuxion logo](https://github.com/anonymousproo/Fix-W-Target-Packages-is-configured-multiple/blob/main/91ecac0b90b912f72ebffa896051adf7.jpg)
# Fix-W-Target-Packages-is-configured-multiple

I just installed Ubuntu Gnome 16.04. I told it to save my documents - which worked. Some software had to be reinstalled. Now when I run sudo apt-get update I see this:

W: Target Packages (main/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-i386/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-i386/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Translations (multiverse/i18n/Translation-en_GB) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Translations (multiverse/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target DEP-11 (multiverse/dep11/Components-amd64.yml) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target DEP-11-icons (multiverse/dep11/icons-64x64.tar) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: The repository 'http://extras.ubuntu.com/ubuntu xenial Release' does not have a Release file.<br>
N: Data from such a repository can't be authenticated and is therefore potentially dangerous to use.<br>
N: See apt-secure(8) manpage for repository creation and user configuration details.<br>
W: http://dl.google.com/linux/chrome/deb/dists/stable/Release.gpg: Signature by key 4CCA1EAF950CEE4AB83976DCA040830F7FAC5991 uses weak digest algorithm (SHA1)<br>
W: http://repo.sinew.in/dists/stable/InRelease: Signature by key B6DA722E2E65721AF54B93966F7565879798C2FC uses weak digest algorithm (SHA1)<br>
E: Failed to fetch http://extras.ubuntu.com/ubuntu/dists/xenial/main/source/Sources  404  Not Found [IP: 91.189.92.152 80]<br>
E: Failed to fetch http://extras.ubuntu.com/ubuntu/dists/xenial/main/binary-amd64/Packages  404  Not Found [IP: 91.189.92.152 80]<br>
E: Failed to fetch http://extras.ubuntu.com/ubuntu/dists/xenial/main/binary-i386/Packages  404  Not Found [IP: 91.189.92.152 80]<br>
E: Some index files failed to download. They have been ignored, or old ones used instead.<br>
W: Target Packages (main/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-i386/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>
W: Target Packages (main/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:33 and /etc/apt/sources.list:87<br>


# Is there an automated way to fix this?

Recent, up-to-date solution

I wrote a Python script to automate this task.

# Installation:

sudo apt install python3-apt

# friest [Download file here](https://github.com/anonymousproo/Fix-W-Target-Packages-is-configured-multiple/raw/main/aptsources-cleanup.pyz)

cd Downloads

sudo chmod +x [file name] ex: aptsources-cleanup.pyz


sudo python3 -OEs [file name] ex: aptsources-cleanup.pyz]
