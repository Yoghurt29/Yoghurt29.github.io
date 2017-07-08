---
layout: post
title: Sample Post
excerpt: "JAVA WEB项目-料件盘点系统"
categories: [project list]
comments: true
image:
  feature: https://images.unsplash.com/photo-1440635592348-167b1b30296f?crop=entropy&dpr=2&fit=crop&fm=jpg&h=475&ixjsv=2.1.0&ixlib=rb-0.3.5&q=50&w=1250
  credit: thomas shellberg
  creditlink: https://unsplash.com/photos/Ki0dpxd3LGc
---
<script>
	alert("js");
</script>
<img src="img/leonids-logo.png"></img>
轮播图片展示项目
## 第一个独立完成的WEB项目
	
	该系统用于盘点生产料件。
	
	###用到的框架
		前端 BootStrap jQuery Echart
		后台 Spring SpringMVC Hibernate
	###主要功能模块特点
	
	*退发料件录入
		使用web socket实现服务器主动推送退发料记录，使得多个用户同时使用时可同步展示库存数据。
	*盘点数据导入导出
		编写Excel读取工具，努力做到使用简单灵活，复用性高。从Excel文件数据读取任意类对象集合，如List<T> List<Map>
	*可视化图表报表
		使用Echart报表生成库，可视化展示后台数据。
	*邮件报告
	*借料签流程单
		实现签核流程定制化功能，用户可配置签核人员节点，定义签核流程。
		
	###