_Ajax-Function
==============

###一个普通的Ajax的构造函数

这玩意就是一函数
原生Ajax写起来太臃肿
自已要做一项目，用不了Jquery，就自已写！


###文档
###1:引用函数即可

###2：初始化函数
//JS
var Get=_Ajax("http://url.com");
//初始化Url,并且存入Url参数


###2：选择传输方法
//JS
Get._get(True);
// _get()方法：只有一个参数，异步或者同步，geturl在初始化的时候就应该选择好

//JS
Get._post("data",True);
//_post()方法:data参数为传输的POST数据,第二个为异步或者同步


###3:获取结果
Get._ok(Function());
//这个我觉得有BUG，但是无大碍！
//传输成功，执行存进来的函数！函数第一个参数是返回的数据
