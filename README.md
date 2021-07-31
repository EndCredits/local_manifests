# local_manifests

Manifests for building Android R on msm8953 platform

If you are building PixelExperience or any other ROM already included those dependencies , please ignore this repository

usage:
```
git clone https://github.com/EndCredits/local_manifests.git -b common-11.0-rebrand .repo/local_manifests
```
### Note:

This local_manifest is made for dotOS building.If you need to compile on other custom rom,please manually change the context in 1_remove.xml.

e.g. (For dotOS)

```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

    <remove-project path="hardware/qcom-caf/msm8996/audio" name="android_hardware_qcom_audio" revision="dot11-caf-msm8996" remote="dot" />
    <remove-project path="hardware/qcom-caf/msm8996/display" name="android_hardware_qcom_display" revision="dot11-caf-msm8996" remote="dot" />
    <remove-project path="hardware/qcom-caf/msm8996/media" name="android_hardware_qcom_media" revision="dot11-caf-msm8996" remote="dot" />
    
</manifest>
```
