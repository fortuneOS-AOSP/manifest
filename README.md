# FortuneOS

# Build guide

Prior to building, you will need basic knowledge of [Git](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet).

### Requirements
- Around 100G disk space.
- A computer with at least 16GB RAM running Linux (recommended) or MacOS.
- Build environment [setup](https://github.com/akhilnarang/scripts).

### Instructions
1. Run the following commands to sync source

```
repo init --no-repo-verify -u https://github.com/fortuneOS-AOSP/manifest.git -b vangelis -g default,-mips,-darwin,-notdefault --git-lfs
```
2. To sync source, enter

```
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```

3. Once the source is downloaded/synced, prepare your device trees, dependencies and start the build by the following commands

```
source build/envsetup.sh
lunch fortune_<devicecodename>-user
mka fortune -j$(nproc --all)
```

## Credits
 * [**AOSP**](https://android.googlesource.com/platform)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**BlissRoms**](https://github.com/BlissRoms)
 * [**crDroid Android**](https://github.com/crdroidandroid)
 * [**DerpFest AOSP**](https://github.com/DerpFest-AOSP)
 * [**Halcyon Project**](https://github.com/halcyonproject)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**Project-Awaken**](https://github.com/Project-Awaken)
 * [**ProtonAOSP**](https://github.com/ProtonAOSP)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**PixelOS**](https://github.com/PixelOS-AOSP)
 * [**PixysOS**](https://github.com/PixysOS)
 * [**RisingOS**](https://github.com/RisingTechOSS)
 * [**StatixOS**](https://github.com/StatiXOS)
 * [**TheParasiteProject**](https://github.com/TheParasiteProject)
 * [**Yet another AOSP project**](https://github.com/Yaap)
 * [**xdroidOSS**](https://github.com/xdroid-oss)
 * [**ManyMore from where cherry-picked from**](https://github.com)
