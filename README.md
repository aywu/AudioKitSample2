This repo provides the fix to one bug (the online playlist cannot be played) in the following repo:
https://github.com/HMS-Core/hms-audio-demo

The fix is to add an attribute:
android:usesCleartextTraffic="true"
to the element "application" in AndroidManifest.xml.

Also, I added the following feature. In the original Audio Kit demo app, when the app goes into
background or exists, the playlist still play uninterrupted. This makes the app behave
strangely. I fixed this issue.

The last problem is that in the original demo codes the online play list contains these play songs:
https://lfmusicservice.hwcloudtest.cn:18084/HMS/audio/Taoge-chengshilvren.mp3
https://lfmusicservice.hwcloudtest.cn:18084/HMS/audio/Taoge-dayu.mp3

cannot be played in North America. I replaced these by the ones that can be played in North America.

Author: Alan Wu
Date: 10/5/2020
