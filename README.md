## TWRP device tree for Intex Aqua Power HD (Aqua_Power_HD)

Add to `.repo/local_manifests/Aqua_Power_HD.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/intex/Aqua_Power_HD" name="android_device_intex_Aqua_Power_HD" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_Aqua_Power_HD-eng
make -j5 recoveryimage
```
