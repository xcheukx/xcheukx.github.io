---
layout: post
title:  "[React Native]Remote debugger提示window找不到chrome"
date:   2017-08-07 16:38:00 +0800
cover: "assets/img/cover/3.png"
tags: [React,前端]
---
先设置默认浏览器为chrome，
然后修改 `node_modules\react-native\local-cli\server\util\lauchChrome.js`
找到 `{app: [getChromeAppName()]}` 修改为 `{}`
重新运行即可