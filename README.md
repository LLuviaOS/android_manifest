# LLuvia OS #

## Setting up your Linux Distribution for Android Compiling: ##
   -  ## Installing Repo ##
   
   ```bash
   # Make a directory where Repo will be stored and add it to the path
   $ mkdir ~/bin
   $ PATH=~/bin:$PATH

   # Download Repo itself
   $ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo

   # Make Repo executable 
   $ chmod a+x ~/bin/repo
   ```
   
   - ## Initializing Repo ##
   
   ```bash
   # Create a directory for the source files
   # You can name this directory however you want, just remember to replace
   # WORKSPACE with your directory for the rest of this guide.
   # This can be located anywhere (as long as the fs is case-sensitive)
   $ mkdir WORKSPACE
   $ cd WORKSPACE

   # Install Repo in the created directory
   # Use a real name/email combination, if you intend to submit patches
   $ repo init -u https://github.com/LLuviaOS/platform_manifest -b 8.1
   ```
   
   - ## Necessary tools/packages to build LLuvia ##
   
   ```bash
   For a debian user:
   sudo apt-get install git-core gnupg flex bison gperf build-essential \
   zip curl zlib1g-dev gcc-multilib g++-multilib libc6-dev-i386 \
   lib32ncurses5-dev x11proto-core-dev libx11-dev lib32z-dev ccache \
   libgl1-mesa-dev libxml2-utils xsltproc unzip \
   curl flex git  libesd0-dev liblz4-tool libncurses5-dev \
   libsdl1.2-dev libwxgtk3.0-dev libxml2  lzop maven pngcrush \
   schedtool squashfs-tools xsltproc zip zlib1g-dev lib32readline6-dev \
   g++-multilib gcc-multilib lib32ncurses5-dev lib32z1-dev openjdk-8-jdk
  
   #maybe in some servers you need bc so do
   sudo aptitude install bc
   
   For an ARCH user:
   lib32-gcc-libs git gnupg flex bison gperf sdl wxgtk2 squashfs-tools curl n
   curses zlib schedtool perl-switch zip unzip libxslt python2-virtualenv 
   bc rsync ncurses5-compat-libsAUR lib32-zlib lib32-ncurses lib32-readline 
   lib32-ncurses5-compat-libsAUR xml2 lzop pngcrush imagemagick
   ```
   
## Building and Support ##

## TO build LLuvia  ##
```bash
   $ . build/envsetup.sh
   $ lunch LLuvia_device-userdebug
   $ lunch #select your device from lunch menu
   $ make rain
   ```
   
## For Official Support ##
- All devices MUST be configured as userdebug releases.
- All devices MUST be configured for SELinux Enforcing.

## our Community ##
Telegram : https://t.me/LLuviaOs
G+ : https://plus.google.com/communities/100235695574462029127?sqinv=TlRpNXYxMUszMDBZdGNxUTVubDNSWkFqbWd4OFlB
