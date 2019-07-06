<p align="center">
<img src="https://github.com/LLuviaOS/XDA-Template/blob/LL-3.1/lluvia.png"> 
</p>

LLuviaOS-X Pie
===========
LLuviaOS stands for Rain in spanish . A rom which is highly optimised and with properly designed User Interface. Primary goal is to provide high performance && best stability of battery .

Credits
-------
* [**JDCTeam**](https://github.com/AOSP-JF-MM)
* [**DirtyUnicorns**](https://github.com/DirtyUnicorns)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Nitrogen Project**](https://github.com/nitrogen-project)
* [**ABC ROM**](https://github.com/ezio84)
* [**GZOSP**](https://github.com/GZOSP)
* [**Pure Nexus**](https://github.com/PureNexusProject)
* [**OmniROM**](https://github.com/omnirom/)
* [**AOSPA**](https://github.com/aospa/)
* [**BlissRoms**](https://github.com/BlissRoms)

How to Build?
-------------

To initialize your local repository using the LLuviaOS trees, use a 
command like this:

```bash
  repo init -u git://github.com/LLuviaOS/android_manifest.git -b LL-3.1
```
To initialize a shallow clone, which will save even more space & time, use a command like this:

```bash
  repo init --depth=1 -u git://github.com/LLuviaOS/android_manifest.git -b LL-3.1
```
  
Then to sync up:
----------------

```bash
  repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------

```bash
  . build/envsetup.sh
  lunch lluvia_device_codename-userdebug
  mka lluvia
```
## Report build issues
- You can reach us via [Telegram](https://t.me/LLuviaOs)

## Maintain Officially
- All devices MUST be configured as userdebug releases.
Build Unofficial and release in xda then apply for official support.
Form: https://goo.gl/forms/lad1qDHLKttcffei2

### Important Links:
- Telegram : https://t.me/LLuviaOs
