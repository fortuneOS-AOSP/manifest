FortuneOS
===========

Getting started
---------------

To get started with Android/FortuneOS, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the FortuneOS trees, use a command like this:
```
repo init -u https://github.com/fortuneOS-AOSP/manifest.git -b vangelis --git-lfs
```
Then to sync up:
```
repo sync
```

Building the System
-------------------
 Initialize the ROM environment with the envsetup.sh script.

```bash
. build/envsetup.sh
```

Lunch your device after cloning all device sources if needed.

```bash
lunch fortune_devicecodename-buildtype
```

Start compilation

```bash
mka fortune
```
