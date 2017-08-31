---
layout: post
title:  "[React Native]遇到的问题记录"
date:   2017-08-09 14:39:00 +0800
cover: "assets/img/cover/3.png"
tags: [React,前端]
---

问：执行`react-native run-android`时，提示`unable to load script from assets index.android.bundle on windows`。

解决方案如下：

1. (项目目录下) `mkdir android/app/src/main/assets`

2. `react-native bundle --platform android --dev false --entry-file index.android.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res`

3. `react-native run-android`

问题就解决好了

问：<Text>文字怎么换行

答：{'\n'} 相当于<br />

问：Unable to process incoming event ‘ProgressComplete ’ (ProgressCompleteEvent)

答：执行 ./gradlew assembleRelease --console plain

