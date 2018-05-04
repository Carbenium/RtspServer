# RtspServer


项目初衷<br>
-
* 一直使用live555做流媒体转发服务，但是live555在嵌入式平台表现不佳，3路1080P并发访问开始出现丢包, 而且音视频不同步。所以自己重新实现了一个RTSP服务器，效果不错，使用方法和live555一样。<br>
* 自己从毕业以来一直想实现一个流媒体服务器, 现在已经走出了第一步。项目目前也还有许多完善的地方, 如果使用的过程中遇到问题, 希望大家可以反馈给我, 谢谢。<br>

目前情况<br>
-
* 支持 Windows 和 Linux平台。
* 支持 H264, H265, G711A, AAC 四种音视频格式的转发。<br>
* 支持同时传输音视频。<br>
* 支持单播(RTP_OVER_UDP, RTP_OVER_RTSP), 组播。<br>

编译环境<br>
-
* Linux: ubuntu16.04 -- gcc4.7<br>
* Windows: win10 -- vs2015<br>

后续计划<br>
-
* 增加其他音视频格式的支持。
* 增加RTCP。
* 其他优化。
 
其他问题<br>
-
* 如何转发媒体文件? 目前没有实现对媒体文件的解析, 可以通过ffmpeg对文件进行帧读取再进行转发。
