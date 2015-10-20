# weibo-android-sdk-core

[![Download](https://api.bintray.com/packages/8tory/maven/weibo-android-sdk-core/images/download.svg) ](https://bintray.com/8tory/maven/weibo-android-sdk-core/_latestVersion)
[![JitPack](https://img.shields.io/github/tag/8tory/weibo-android-sdk-core.svg?label=JitPack)](https://jitpack.io/#8tory/weibo-android-sdk-core)
[![Build Status](https://travis-ci.org/8tory/weibo-android-sdk-core.svg)](https://travis-ci.org/8tory/weibo-android-sdk-core)

![](art/weibo-android-sdk-core.png)

Used to integrate Android apps with Weibo Platform.

Import from https://github.com/sinaweibosdk/weibo_android_sdk/releases

## Installation

via jcenter:

```gradle
repositories {
    jcenter()
}

dependencies {
  compile 'com.infstory:weibo-android-sdk-core:3.1.2'
}
```

or, via jitpack:

```gradle
repositories {
    jcenter()
    maven { url "https://jitpack.io" }
}

dependencies {
  compile 'com.github.8tory:weibo-android-sdk-core:-SNAPSHOT'
}
```

## Build

debug:

```sh
./gradlew assembleDebug
```

release and deploy:

~/.gradle/gradle.properties

```
NEXUS_USERNAME=X+XXX
NEXUS_PASSWORD=zXX/+XXX

signing.keyId=XXX
signing.password=XXX
signing.secretKeyRingFile=/home/andrew/.gnupg/secring.gpg

DEBUG_PASSWORD=XXX

BINTRAY_USER=yongjhih
BINTRAY_KEY=XXX
```

```sh
./gradlew clean build bintrayUpload
```

## See Also

* https://github.com/8tory/weibo-android-sdk

jar md5sum:

```
67e5d04955b6cb00b4edec31e3b85276  weiboSDKCore_3.1.2.jar (90483510, non-github-release-3.1.2)
dd7eae7d2308aa503f48b358da40e69e  ./weibo_android_sdk-3.1.1/weibosdkcore_v3.1.1.jar
a8ecaf0e017737cdc4898077b98d2be2  ./weibo_android_sdk-3.0.1/weibosdkcore_v3.0.1.jar
67f223b3d92fffe77df2984b49ca104e  ./weibo_android_sdk-2.5.1/weibosdkcore.jar
84b92e8ced6db809f47cb85d54708a4b  ./weibo_android_sdk-2.5.0/weibosdkcore.jar
f830c348e1fb80558fdc6d24ed1d65f4  ./weibo_android_sdk-2.4.0/weibosdkcore.jar
30eb234e7863336fdae186628be49ad5  ./weibo_android_sdk-2.3.0/weibo_sdk.jar
```

so md5sum, v3.1.2 (90483510):

```
054ed4f4db34a831eab581e88d7fb21d  ./libs/arm64-v8a/libweibosdkcore.so
165db49643709f9fb0fe6b9d475c4329  ./libs/armeabi/libweibosdkcore.so
7c20bf0ce30ffb6fc1cfe161738ad0b7  ./libs/x86_64/libweibosdkcore.so
7ad9588163f82ac0dc55f8d12816d817  ./libs/armeabi-v7a/libweibosdkcore.so
bda1b819f07ba096ad1fb087208d9717  ./libs/x86/libweibosdkcore.so
c44e7b9f55b889bde5cdb66437e3ea14  ./libs/mips64/libweibosdkcore.so
9a8a2e8b46024c671da423fb35a33ee2  ./libs/mips/libweibosdkcore.so

054ed4f4db34a831eab581e88d7fb21d  ./demo-src/WeiboSDKDemo/libs/arm64-v8a/libweibosdkcore.so
165db49643709f9fb0fe6b9d475c4329  ./demo-src/WeiboSDKDemo/libs/armeabi/libweibosdkcore.so
7c20bf0ce30ffb6fc1cfe161738ad0b7  ./demo-src/WeiboSDKDemo/libs/x86_64/libweibosdkcore.so
7ad9588163f82ac0dc55f8d12816d817  ./demo-src/WeiboSDKDemo/libs/armeabi-v7a/libweibosdkcore.so
bda1b819f07ba096ad1fb087208d9717  ./demo-src/WeiboSDKDemo/libs/x86/libweibosdkcore.so
c44e7b9f55b889bde5cdb66437e3ea14  ./demo-src/WeiboSDKDemo/libs/mips64/libweibosdkcore.so
9a8a2e8b46024c671da423fb35a33ee2  ./demo-src/WeiboSDKDemo/libs/mips/libweibosdkcore.so
```

## License

```
Copyright 2015 8tory, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
