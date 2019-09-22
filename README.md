# LLuviaOS #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/LLuviaOS/android_manifest -b LL-4.X

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch lluvia_$device-userdebug

# Build the code
$ mka storm -jX
```