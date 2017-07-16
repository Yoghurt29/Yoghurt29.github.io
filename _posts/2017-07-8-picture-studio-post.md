---
layout: post
title: 投影图片工作室（JAVA Swing应用）
excerpt: "桌面应用，可将用户给定的矢量图等通过投影仪输出到地面。用于辅助定位。;"
categories: [about Trulon]
comments: true
image:
  feature: #https://images.unsplash.com/photo-1440635592348-167b1b30296f?crop=entropy&dpr=2&fit=crop&fm=jpg&h=475&ixjsv=2.1.0&ixlib=rb-0.3.5&q=50&w=1250
  credit: thomas shellberg
  creditlink: https://unsplash.com/photos/Ki0dpxd3LGc
---
<img src="img/picture_studio_main_view.png" >
<img src="img/picture_studio_work_view.png" >

##需求功能
* 支持AI等矢量图，
	使用JAVA语言调用脚本库，实现矢量图格式到普通格式的转换
* 可扫描图像线框，
	使用OPENCV提供的函数扫描出图片
* 可选择裁切范围，
	类似于截图工具可选择范围
* 校准投影距离参数后可指定输出到地面的图像大小。