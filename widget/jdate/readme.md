# 功能描述

   多格式、功能强大的移动端日期选择插件
	

# 快速使用
	调用jdate.min
	<script type="text/javascript" src="libs/jdate.min.js"></script>

	存放时间的位置
	例1：
	<div class="form-group clearfix">
		<div class="col-xs-6">
			<input readonly class="form-control" type="text" id="date-group1-1" placeholder="YYYY-MM">
		</div>
		<div class="col-xs-6">
			<input readonly class="form-control" type="text" id="date-group1-2" placeholder="YYYY-MM-DD">
		</div>
	</div>
	

	js调用插件
	// 格式
		new Jdate({
			el: '#date-group1-1',
			format: 'YYYY-MM',
			beginYear: 2000,
			endYear: 2100
		})
		new Jdate({
			el: '#date-group1-2',
			format: 'YYYY-MM-DD',
			beginYear: 2000,
			endYear: 2100
		})

	例2：
	<div class="form-group clearfix">
		<div class="col-xs-6">
			<input readonly class="form-control" type="text" id="date-group2-1" placeholder="完整实例">
		</div>
	</div>
	
	js调用插件
		
	/* 回调函数
	 * tips:	在vue及其他mvvm框架中使用时，在confirm中修改v-model绑定的数据即可
	 */
	new Jdate({
		el: '#date-group2-1',
		format: 'YYYY-MM-DD',
		beginYear: 2000,
		endYear: 2100,
		init: function() {
			console.log('插件开始触发');
		},
		moveEnd: function() {
			console.log('滚动结束');
		},
		confirm: function(date) {
			console.log(date)
			console.log('确定按钮触发');
		},
		cancel: function() {
			console.log('插件运行取消');
		}
	})
# 特别说明
	html页面中存放的id都有对应的js调用后面跟有注释。
	
	