---
title: OBS设置教程v1.0
date: 2021-04-10 15:44:41
tags: OBS
---

<h1>OBS设置教程v1.0</h1>

<b ><span class="label label-info" style = "font-size:24px ;color:#f01159">OBS并不是一个安装即用的软件</span></b>

<H2><p class="note note-warning" style = "font-size:22px">一、直播设置</p></H2>



1.顶部菜单：配置文件>重命名或者新建并命名配置文件<span class="label label-danger">(如果你只使用一个直播间请跳过此步)</span>

2.左下角：来源添加你需要的项，一般需要添加<span class="label label-success">显示器采集和视频采集设备</span>,对应的是<span class="label label-success">电脑桌面和摄像头(一般是)</span>

<img src="https://i.loli.net/2021/04/10/UryWGOH5d8MEtcz.png" style="zoom:100%;" />

</br>

</br>

3.设置>推流>自定义>填入<span class="label label-success">推流地址和串流密钥(根据实际情况)</span>

<img src="https://i.loli.net/2021/04/10/4D8mydAeUFOZBcJ.png" style="zoom:35.7%;" />

</br>

</br>

4.输出>高级>串流>编码器><span class="label label-danger">x264(不推荐使用，会占用大量CPU资源)</span>/<span class="label label-success">NVIDIA NVENC H.264(优先推荐使用)</span><span class="label label-warning">根据GPU的不同可能是其他名称，尽量不要使用x264</span>

码率控制><span class="label label-warning">CBR(固定码率)</span>/<span class="label label-danger">CQP(恒定质量参数，不推荐使用，除非你了解这是什么)</span>/<span class="label label-success">VBR(动态码率，推荐)</span>/<span class="label label-primary">无损(只要设备、带宽够好)</span>>比特率>500kbps(直播偏静态画面) ~ ∞(直播偏动态画面)>其他默认，除非你知道那些设置是什么

<img src="https://i.loli.net/2021/04/10/XGBljmSILrQFevf.png" style="zoom:43.8%;" />

</br>

</br>

5.音频><span class="label label-success">绿色框里如图所示设置</span>><span class="label label-danger">红色框里根据自己的需要设置</span>><span class="label label-warning">橙色框一般默认</span>

<img src="https://i.loli.net/2021/04/10/XiYsh2tveKH1B9Z.png" style="zoom:43.8%;" />

</br>

</br>

6.视频><span class="label label-success">绿色框里一般如图所示设置</span>><span class="label label-danger">红色框里根据自己的需要设置</span>

<img src="https://i.loli.net/2021/04/10/7Cnv5pdXus2TWQy.png" style="zoom:43.8%;" />

</br>

</br>

7.到这里就可以开始直播了

</br>

</br>

----------------------------------------

<h2><p class="note note-info" style = "font-size:22px">二、录屏设置</p></h2>

<span class="label label-info">第1、2步设置</span> 同 <span class="label label-warning">直播设置第1、2步</span>一样

3.输出>高级>类型>标准>录像路径径(自定义)><span class="label label-success">录像格式(推荐mkv，意外关机的情况下，可保留关机前录制的视频文件)</span>><span class="label label-info">编码器、速率控制、比特率设置 </span> 同  <span class="label label-warning">直播设置一样</span>

<img src="https://i.loli.net/2021/04/12/ViSdauyHGWA4Jls.png" style="zoom:44%;" />

</br>

</br>

4、5：<span class="label label-info">音频和视频设置</span> 同 <span class="label label-warning">直播音频和视频设置设置</span>一样

6：如果录制格式使用的是MKV，由于目前大部分后期软件和播放器不支持MKV封装格式，需要转换成MP4封装

左上角菜单 文件>录像转封装

<img src="https://i.loli.net/2021/04/12/DQuitNfIFwXTjUR.png" style="zoom:47.5%;" />

</br>

</br>

点击三个点图标>选择需要转换封装的视频>转换封装(转换完封装的视频文件在原视频同目录下)

<img src="https://i.loli.net/2021/04/12/SvGHYWUhV5uafRi.png" style="zoom:51%;" />