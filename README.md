# jquery.mousewheel 使用介绍

jQuery Mousewheel Plugin,用于添加跨浏览器的鼠标滚轮支持。


> mousewheel事件的处理函数有一点小小的变化，它除了第一个参数event 外，还接收到第二个参数delta。
> 通过参数delta可以获取鼠标滚轮的方向和速度。
> 如果delta的值是负的即-1，那么滚轮就是向下滚动，正的1就是向上。


	// using bind
	$('#my_elem').bind('mousewheel', function(event, delta, deltaX, deltaY) {
	    if (window.console && console.log) {
	         console.log(delta, deltaX, deltaY);
	    }
	});
	// using the event helper
	$('#my_elem').mousewheel(function(event, delta, deltaX, deltaY) {
	    if (window.console && console.log) {
	         console.log(delta, deltaX, deltaY);
	    }
	});