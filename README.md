# fortuneOS

 Getting Started
---------------
To get started with the fortuneOS sources, you'll need to get
familiar with [Git and Repo](https://source.android.com/setup/build/downloading).

 To initialize your local repository, use command:

```bash
repo init -u https://github.com/fortuneOS-AOSP/manifest.git -b usagi --git-lfs
```

Then sync up:

```bash
repo sync -c --force-sync --no-clone-bundle --no-tags -j$(nproc --all)
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
