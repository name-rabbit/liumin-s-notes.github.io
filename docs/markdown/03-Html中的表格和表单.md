# HTML 中的表格和表单

## HTML 中的表格

### 创建一个表格

	<table border="" cellspacing="" cellpadding="" width="" height="">
		<caption>表格标题</caption>
		<tr>
			<th>Header</th>
		</tr>
		
		<tr>
			<td>Data</td>
		</tr>
	</table>
	
	表格由 <table> 标签来定义。
	每个表格均有若干行（由 <tr> 标签定义）
	每行被分割为若干单元格（由 <td> 标签定义）
	字母 th 指表头数据
	字母 td 指表格数据（table data），即数据单元格的内容
	
	表格的表头使用 <th> 标签进行定义
	大多数浏览器会把表头显示为粗体居中的文本
	
	数据单元格可以包含文本、图片、列表、段落、表单、水平线、表格等等
	
	table 的属性值
		border : 设置表格最外部的框框
		width : 设置表格整体的宽度
		height : 设置表格整体的高度
		cellspacing : 单元格外边距
		cellpadding : 单元格内边距
	
	tr 的属性值
		height : 单元格的高度
		align: 单元格内容的水平对齐方向 left左/right右/center居中 
		valign: 文字垂直对齐方式
		
	td 的属性值
		width : 单元格的宽度,一般不去设置，会有新的问题出现
		height : 单元格的高度
		align: 单元格内容的水平对齐方向 left左/right右/center居中 
		colspan : 向右合并单元格(跨列合并)
		rowspan : 向下合并单元格(跨行合并)

## HTML 中的表单

### 表单是什么

	对于用户而言是数据的录入和提交的界面
	对于网站而言获取用户信息的途径

### 创建一个表单

	<form action="" method="" name="">
	
	</form>
	
	action: 定义表单最终提交的地址
	method:	设定数据提交方式，用于根据不同的数据需求来选择合适的提交方式 xxx
		常见的提交方式有：GET,POST 
		GET 和 POST 的区别？
	name: 给表单一个名字，使其成为独一无二的表单 xxx

### 常用的表单元素

	<input type="" value="" name="" placeholder=""/>
	
	type : 类型 默认是 text 文本框 / password 密码框
			/ button 常规按钮 / submit 提交按钮 / reset 重置按钮
			
			/ checkbox 复选按钮 / radio 单选按钮 （是一组选择项，只能选择其中一个，用 name 控制组） xxx
	value : 值
	placeholder : 提示文本
	
	当 value 和 placeholder 属性值 同时存在时，显示 value 的属性值
	
	这表单长得也太丑了吧，怎么能让它变的好看一点呢？（师生互动）
	设计，加点样式。。。。