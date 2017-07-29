## TWRP device tree for Acer Liquid Z520 (acer_Z520)

Add to `.repo/local_manifests/acer_Z520.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/acer/acer_Z520" name="android_device_acer_acer_Z520" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_acer_Z520-eng
make -j5 recoveryimage
```
