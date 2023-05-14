# CHRISL7_fog
## Easy clone
Firts U need init repo the ROM u want, example:
```
repo init -u https://github.com/Project-Awaken/android_manifest -b triton --git-lfs
```
Clone the trees on repo 
```
git clone https://github.com/Joxquin/CHRISL7_fog.git --depth 1 -b main .repo/local_manifests
```
Now sync the source
```
repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```
Done!

## Source commit dependencies:
- vendor/aosp: https://github.com/PixelExperience/vendor_aosp/commit/97c0cd376fc1f160664d29e3a8e5f4559a9a53b0
- vendor/aosp: https://github.com/PixelExperience/vendor_aosp/commit/6a23cfd3ad4ac795eb4fe0559dc6ac2b5b6ce505
- vendor/qcom/opensource/interfaces: https://github.com/PixelExperience/vendor_qcom_opensource_interfaces/commit/0a1e8499b11c9c80a58510faa7f63e2d85ab831d
- vendor/qcom/opensource/fm-commonsys: https://github.com/PixelExperience/vendor_qcom_opensource_fm-commonsys/commit/811cd5b96868d944572b2bd28b8740a6e8e90725

### QCOM/COMMON adaptations:
#### Adapt these paths to your rom:
- https://github.com/PixelExperience-Devices/device_qcom_common-sepolicy/commit/4ae0e346edb8c1525d3d86bc07bcedb312fbf74c
- https://github.com/PixelExperience-Devices/device_qcom_common/commit/3802e110b09081fc259af9438096801e8c39cd4b
