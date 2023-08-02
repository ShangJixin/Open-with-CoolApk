# Open-with-CoolApk
Open with CoolApk / 用酷安打开

插件在[GreasyFork](https://greasyfork.org/zh-CN/scripts/472260)发布，Github作为备份使用。

Release at [GreasyFork](https://greasyfork.org/zh-CN/scripts/472260). This repo is a backup.

解决酷安网页分享链接无法在Windows浏览器下拉起WSA版酷安的问题。

Fix URL Scheme function model to open CoolApk's Share link with CoolApk'APP in WSA(Windows Subsystem for Android).

通过看代码，发现了酷安其实是对Android版进行适配了，使用的是唤起intent的方式。iOS/iPadOS不太清楚技术细节，但看样子是引导用户前往App Store，且经过测试URL Scheme无法在iOS端使用。

但URL Scheme在安卓端也是有用的，在电脑网页端拉起酷安WSA时也是有用的，故基于酷安官方分享链接网页里的JavaScript代码进行修改，最终实现了可以在电脑可以方便的使用酷安的分享链接。
