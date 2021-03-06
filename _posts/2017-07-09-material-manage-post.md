---
layout: post
title: 料件盘点系统
excerpt: "使用BootStrap Echart呈现前端数据页面,使用ajax异步交互获取数据,使用SpringMVC Hibernate支撑后台业务;"
categories: [project list]
comments: true
image:
  feature: #https://images.unsplash.com/photo-1440635592348-167b1b30296f?crop=entropy&dpr=2&fit=crop&fm=jpg&h=475&ixjsv=2.1.0&ixlib=rb-0.3.5&q=50&w=1250
  credit: thomas shellberg
  creditlink: https://unsplash.com/photos/Ki0dpxd3LGc
---
<div id="myCarousel" class="carousel slide">
	<!-- 轮播（Carousel）指标 -->
	<ol class="carousel-indicators">
		<li data-target="#myCarousel" data-slide-to="0" id="slide-to0" class="active"></li>
		<li data-target="#myCarousel" data-slide-to="1" id="slide-to1"></li>
		<li data-target="#myCarousel" data-slide-to="2" id="slide-to2"></li>
		<li data-target="#myCarousel" data-slide-to="3" id="slide-to3"></li>
	</ol>   

	<!-- 轮播（Carousel）项目 -->
	<div class="carousel-inner">
		<div class="item active">
		<img src="img/material_manage_day_data_view.png" alt="First slide">
		</div>
		<div class="item">
		<img src="img/material_manage_back_line_chart_view.png" alt="Second slide">
		</div>
		<div class="item">
		<img src="img/material_manage_manage_material_view.png" alt="Third slide">
		</div>
		<div class="item">
		<img src="img/material_manage_sign_order_view.png" alt="fourth slide">
		</div>
	</div>
	<!-- 轮播（Carousel）导航 -->
	<a class="carousel-control left" href="#myCarousel" data-slide="prev">‹</a>
	<a class="carousel-control right" href="#myCarousel" data-slide="next">›</a>
</div>

<!-- 控制按钮 -->
<br>
<div style="text-align:center;">
	<input type="button" class="btn slide-one" value="首页">
	<input type="button" class="btn slide-two" value="图表展示">
	<input type="button" class="btn slide-three" value="数据维护">
	<input type="button" class="btn slide-fourth" value="签单界面">
</div>
<div id="projectDetail">
	<h2> 第一个独立完成的WEB项目</h2>
	
	<p>该系统用于盘点生产料件。</p>
	
	<h3>使用的框架</h3>
	<ul>
		<li>前端 BootStrap jQuery Echart</li>
		<li>后台 Spring SpringMVC Hibernate</li>
	</ul>	
	<h3>主要功能模块特点</h3>
	<ul>
		<li>
			<h5>
				退发料件录入
			</h5>
			<p>
				使用web socket实现服务器主动推送退发料记录，使得多个用户同时使用时可同步展示库存数据。
			</p>
		</li>
		<li>
			<h5>
				盘点数据导入导出
			</h5>
			<p>
				编写Excel读取工具，努力做到使用简单灵活，复用性高。从Excel文件数据读取任意类对象集合，如List&lt;T&gt; List&lt;Map&gt;
			</p>
		</li>
		<li>
			<h5>
				可视化图表报表
			</h5>
			<p>
				使用Echart报表生成库，可视化展示后台数据。
			</p>
		</li>
		<li>
			<h5>
				邮件报告
			</h5>
			<p>
				实现将前台Echart生成的图表传到后台，放到邮件正文中。
			</p>
		</li>
		<li>
			<h5>
				借料签流程单
			</h5>
			<p>
				实现签核流程定制化功能，用户可配置签核人员节点，定义签核流程。
			</p>
		</li>
	</ul>
</div>	
<link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css">
<script src="https://cdn.bootcss.com/jquery/2.1.1/jquery.min.js"></script>
<script src="https://cdn.bootcss.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
<script>
	$(function(){
		// 初始化轮播
			//$("#myCarousel").carousel('cycle');
		// 停止轮播
			//$("#myCarousel").carousel('pause');
		// 循环轮播到上一个项目
			//$("#myCarousel").carousel('prev');
		// 循环轮播到下一个项目
			//$("#myCarousel").carousel('next');
		// 循环轮播到某个特定的帧 
		$(".slide-one").click(function(){
			$("#myCarousel").carousel(0);
			$("#slide-to0").click();
		});
		$(".slide-two").click(function(){
			$("#myCarousel").carousel(1);
			$("#slide-to1").click();
		});
		$(".slide-three").click(function(){
			$("#myCarousel").carousel(2);
			$("#slide-to2").click();
		});
		$(".slide-fourth").click(function(){
			$("#myCarousel").carousel(3);
			$("#slide-to3").click();
		});
	});
</script>