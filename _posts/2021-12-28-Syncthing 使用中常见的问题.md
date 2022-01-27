---
layout: mypost
title: Syncthing 使用中常见的问题
categories: [杂文]
---

安卓手机端同步目录提示 错误 (folder marker missing)
这是由于该同步目录下面缺少一个 .stfolder 目录，解决办法是在该目录下新建文件夹:.stfolder (注意前面的 ".")，因为该文件夹为隐藏文件夹，有的国内定制安卓系统或者系统清理软件会自动清除该文件夹，所以如果新建 .stfolder 文件夹后还出现这样的情况，可以在 .stfolder 里随便新建一个空文件，比如我就在该文件夹下新建一个名为 .stfolder 的空文件。
Windwos 端 SyncTranyzor 提示升级, 但是每次升级会没反应或提示 upgrade already in progress 或 An existing connection was forcibly closed by the remote host
刚开始错误的以为是 SyncTranyzor 需要升级,，实际上是 Syncthing 需要升级，关闭 SyncTranyzor ，将官网的 Syncthing.exe 文件复制到 C:Users用户名AppDataRoamingSyncTrayzor 目录下，覆盖原文件既可。
安卓的 Syncthing 耗电太猛
安卓端 Syncthing 因为需要实时监控文件变化，所以耗电挺猛，这个需要等软件优化，目前先设置成只在充电的时候开启自动同步既可。
