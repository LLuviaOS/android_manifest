# LLuviaOS-Pie
<p align="center">
  <img width="300" height="300" src="https://github.com/LLuviaOS/XDA-Template/blob/lluvia-2.x/img/lluvia_3.x.png">
</p>

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
   $ repo init -u https://github.com/LLuvia-OS/android_manifest -b 3.0
   
   # To sync lluvia repo
   $ repo sync -c -f --force-sync --no-tags --no-clone-bundle -j8
   ```
   
## Building and Support ##

## TO build LLuvia  ##
```bash
   $ . build/envsetup.sh
   $ lunch #select your device from lunch menu (or) lluvia_device-userdebug
   $ time mka rain
   ```
   
## For Official Support ##
- All devices MUST be configured as userdebug releases.
- All devices MUST be configured for SELinux Enforcing.

## Our Community ##
- Telegram : https://t.me/LLuviaOs
- G+ : https://plus.google.com/communities/100235695574462029127?sqinv=TlRpNXYxMUszMDBZdGNxUTVubDNSWkFqbWd4OFlB
