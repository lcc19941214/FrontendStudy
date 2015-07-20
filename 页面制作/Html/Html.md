#html标签
##常用属性/全局属性
+ id
+ class
+ style
+ title
	
##标签大致分类
<blockquote>
	+ 文档标签/章节标签
	+ 标题标签
	+ 文本标签
	+ 组合内容
	+ 资源标签	 
	+ 表格标签
	+ 表单标签
	+ 实体字符
</blockquote>
		
###文档标签    `参考命名规范——如NEC`
- body
- header
- nav 
- article
- section
- aside
- footer
		
###标题标签
- h1,h2,h3,h4,h5,h6
		
###文本标签

- <a>  
>指向一个链接 `<a href:"http://www.w3c.com>click</a>`

>指向一个锚点 `<a href:"#p1">click</a>`

>		`<div id="#p1">here</div>`

>链接到邮件   `<a href:"mailto:123@456.com">mail me</a>`

>		`target: _blank _self FrameName`(框架的名称，可以直接跳转到框架)

- 强调 `<strong>`  重要性上

	`<em>`  语义上
	
- `<br />`

- 引用 `<cite>`
	`<q>`
	 `<blockquote>`

- 代码 `<code>`

- 格式化 `<b> <i> <u> <s> <sub> <sup>`
		
###组合内容

- 分区 `<div>`  
> //block,默认宽度是父元素宽度

- 段落 <p>     
>//block
	
- 列表 
+ `<ul><ol><li>` 
+ `<dl><dt><dd>`
> //li和dd存在的缩进，可用 margin-left=0清除

- pre  保留文本格式
> //参见css white-space
> //pre会使得font-family设置无效
		
###资源标签
- `<img>`
- `<iframe>` //框架
- `object` `embed` 嵌入外部资源
	> `<object></object>`
	> `<embed />`
			
	> <object date="xxx.mp3" type="--/--">
			</object>
			
	>	`<embed src="xxx.mp3" />`
- video
	>	`<video 	controls	autoplay	 loop 	poster="../images/poster.jpg"	width height>`

				控制条	自动播放	循环播放	第一帧图片	宽高
				
				<source src="xxx.mp3" type="video/mp4" />
				
				<source src="xxx.mp3" type="video/mpeg" /> //兼容
				
				<source src="xxx.mp3" type="video/avi" /> //兼容
				
				<track kind="subtitles" src="./res/video.vtt" srclang="cn" label="cn"></track>
				
			</video>
- audio
			//type="video/mp4"
			//type="audio/mp3"
		
- 嵌入资源
		·图  -canvas    绘制函数/场景复杂    像素
			-svg      高保真/静态/图形图像  矢量
			
		·热点  -map
			 -area
				<area
					shape="rect/circle/poly"
					coords="x1,y1,x2,y2/x,y,r/x1,y1,x2,y2,x3,y3……"
					target="_blank"
					alt="xxx"
					href="http://"
					/>
					
###表格标签
- table
>	`<table>`

>		`<thead>`

>			`<tr>`

>				`<th>`

>		`<tbody>`

>			`<tr>`

>				`<td>`

>		`<tfoot>`

>			`<tr>`

>				`<td>`
	
- 行、列合并
			colspan  跨列

			rowspan  跨行
			
###表单标签
- `<input>`  name//提交的值的名称
	value//提交的值
	text	password	radio	checkbox	button	submit
	files	images	hidden	reset		
- `<select>`
`<opgroup>`
`<option>`
			
- `<textarea>`
resize:none  //文本框拖拽
		
- `<fieldset>`
`<legend>`
			
>     属性
			placeholder //placeholder="请输入用户名”
			readonly //只读
			disable  //无法操作
			checked
			selected
			resize
			
###实体字符
>`空格 &nbsp;  &#160;`
>`引号 &quot;  &#34;`
>`<   &lt;  &#60;`
>`>   &gt;  &#62;`
>`&   &amp; &#38;`
>`版权 &copy;  &#169;`
