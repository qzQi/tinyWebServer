# IncompleteWebServer      
2021/10/28：先记录下吧。      

这个名字（真想换了），一开始觉得写这个挺easy的，后来实现就QWQ了。    



~~和名字一样一个功能不完备的webserver，初步计划仅仅支持get请求。~~    
嗯，在真正开始写才发现在脑海里面构建一个与真正的自己通过代码来实现出来的差距，认真的完成它。




### 步奏
* 1、先完成基本的多线程部分的封装
* 2、写一个基本的线程安全的日志模块

嗯，上面算是模仿muduo的结构吧，上面完成后开始我们网络模块的编写。

这部分的话，之前也看过一些httpServer的写法。觉得没太多的东西，决定也是仿照muduo的写法使用
`one loop per thread`的模型。     
线程模型就做成multiple Reactors+ threadPool的形式。          


计划：      
* 完成基本的Reactor结构
* 添加网络的基本模块

### 进度
* 10/29：完成线程相关类的封装。完成后写线程池的测试程序。
    明天再完善一下。   


### 