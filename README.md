1.canvas中getImageData()跨域问题； 
   同源策略的限制，将图片放入服务器中遵循同源策略即可。

2.github操作
    git init //把这个目录变成Git可以管理的仓库
　　git add README.md //文件添加到仓库
　　git add //不但可以跟单一文件，还可以跟通配符，更可以跟目录。一个点就把当前目录下所有未追踪的文件全部add了 
　　git commit -m "first commit" //把文件提交到仓库
　　git remote add origin git@github.com:wangjiax9/practice.git //关联远程仓库
　　git push -u origin master //把本地库的所有内容推送到远程库上
3.AJAX中http请求动作	
   a、http请求的方法（get/post）或‘动作’
   b、正在请求的url
   c、一个可选的请求头集合，其中可能包括身份验证信息
   d、一个可选的请求主体(get请求没主体)
 服务器返回的http响应包含3部分
   a、一个数字和文字组成的状态码，用来显示请求的成功和失败
   b、一个响应头集合
   c、响应主体
4.linux下的系统管理
   进程管理：
        进程的查看：ps aux 查看系统中所有进程，使用BSD操作系统格式
	            ps -le 查看系统中所有进程，使用Linux标准命令格式
        查看系统健康状态：top
	进程的结束：kill
   进程优先级的修改：ps -le后，修改NI值，PRI（最终值）=PRI（原始值）+NI，越小越优先
	nice命令：给新执行的命令直接赋予NI值，但是不能修改已经存在进程的NI值
	renice命令：修改已经存在进程的NI值命令
   系统资源查看：
	vmstat [刷新延时 刷新次数]：内存实时监控
	free命令查看内存使用状态
	uptime命令，显示系统的启动时间和平均负载
   系统定时任务
	at一次性定时任务：at [选项] 时间 
	crontab循环定时任务
	系统的crontab设置
	anacron配置：anacron是用来保证在系统关机的时候错过的定时任务，可以在系统开机之后再执行

5.JavaScript split() 方法：用于把一个字符串分割成字符串数组。并将结果放在一个数组中
		join()方法：将一个数组合并成一个字符串

6.移动端js触摸(touch)事件
    touchstart   //手指刚接触屏幕时触发
    touchmove    //手指在屏幕上移动时触发，在这个事件发生期间，调用preventDefault()事件可以阻止滚动。
    touchend     //手指从屏幕上移开时触发

    每个Touch对象包含的属性如下：
　　clientX：触摸目标在视口中的x坐标。
　　clientY：触摸目标在视口中的y坐标。
　　identifier：标识触摸的唯一ID。
　　pageX：触摸目标在页面中的x坐标。
　　pageY：触摸目标在页面中的y坐标。
　　screenX：触摸目标在屏幕中的x坐标。
　　screenY：触摸目标在屏幕中的y坐标。
　　target：触目的DOM节点目标。

    三个用于跟踪触摸的属性：
    touches：表示当前跟踪的触摸操作的touch对象的数组。
　　targetTouches：特定于事件目标的Touch对象的数组。
　　changeTouches：表示自上次触摸以来发生了什么改变的Touch对象的数组。
	
