# TWRP Device Tree for Samsung Galaxy S20 FE

The Galaxy S20 FE (codenamed _"r8s"_) is an upper-midrange smartphone from Samsung.

It was announced and released in October 202

## Device specifications

| Feature                      | Specification                                                                      |
| ---------------------------: | :----------------------------------------------------------------------------------|
| Chipset                      | Exynos 990/9830                                                                    |
| CPU                          | Octa-core (2x2.73 GHz Mongoose M5 & 2x2.50 GHz Cortex-A76 & 4x2.0 GHz Cortex-A55)  |
| GPU                          | Mali-G77 MP11                                                                      |
| Memory                       | 6GB/8GB RAM                                                                        |
| Shipped OS                   | Android 10 (One UI 2.0)                                                            |
| Storage                      | 128GB / 256GB (UFS 3.1)                                                            |

## Kernel source 

Available at [https://github.com/ExtremeXT/android_kernel_samsung_990/](https://github.com/ExtremeXT/android_kernel_samsung_990)

## Bugs

- ADB when MTP is disabled
- /data decryption

## How to build

This device tree was tested and is fully compatible with [minimal-manifest-twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).

1. Set up the build environment following the instructions [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-12.1/README.md#getting-started)

2. In the root folder of the fetched repo, clone the device tree:

```bash
git clone https://github.com/ExtremeXT/android_device_samsung_r8s.git -b android-12.1 device/samsung/r8s
```

3. To build:

```bash
. build/envsetup.sh
lunch twrp_r8s-eng
mka recoveryimage
```

## Copyright

```
#
# Copyright (C) 2024 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
```
