### Usage

#### Import

```py
from aapt import aapt, APK
```
1. #### Print `aapt` output
    ```py
    for line in aapt('/path/to/file.apk'):
        print(line)
    ```
2. #### Make an `APK` object
    ```py
    apk = APK('/path/to/file.apk')

    print(apk.package_name)         # com.zhinglong.android.tiktube
    print(apk.version_name)         # 0.69.420
    print(apk.version_code)         # 1234567890
    print(apk.target_sdk_version)   # 26
    print(apk.app_label)            # TikTube
    print(apk.app_icon)             # path/to/some_icon.xml

    print(apk)                      # TikTube
                                    # com.zhinglong.android.tiktube
                                    # 12.34.56

    ```
#### Directory
```py
# Linux
/bin/linux/aapt_64

# Windows
/bin/win32/aapt_64

# Mac OS
/bin/darwin/aapt_64
```