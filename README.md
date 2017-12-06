## TWRP device tree for Samsung Galaxy Note 4 (Snapdragon)
## trltexx, trltedt, trltetmo, trltecan, trltespr, trlteusc, trltevzw

Add to `.repo/local_manifests/trlte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="ripee/android_device_samsung_trlte" path="device/samsung/trlte" remote="github" revision="android-7.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_trlte-eng
mka recoveryimage
```

