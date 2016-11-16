## 播放器api 

### 播放器初始化参数
| 参数 |	值类型	| 说明|	默认值|	是否必填|
| :---: | :---: | :--- | :---: | :---: |
| width |	Number | 播放器宽度，单位是px	|H5播放器是屏幕宽度，flash播放器是840px |	否 |
| height |	Number |	播放器高度，单位是px|	H5播放器是屏幕宽度的9/16，flash播放器是480px |	否 |
| wrapElemId |	String|	父容器ID，包裹播放器的DOM标签ID名称	| 无|	是 |
| type | Number| 	调用类型：0为自适应移动端或PC端，1为调用H5播放器，2为调用flash播放器| 	无	| 是|
| liveId| 	String| 	直播ID| 	无| 	是|
| videoType| 	Number| 	调用类型：1为直播，2为点播	 |无 |	是 |
| videoUrl| 	String或者Array| 	各个模式中都可用String；在移动端点播可使用Array型，代表两个视频，后一个为备用视频地址| 	无|	是 |
| imageUrl| 	String| 	播放器的预览图片地址| 	无| 	是|
| auto	| Boolean| 	调用类型：true为自动播放，false不自动播放（部分手机不支持自动播放）| 	false| 	是|
| xmlid| 	String| 	Flash播放器调用远程的调用接口（Flash播放器专用）| 	无| 	否|
| detailHref| 	String| 	详情链接（h5播放器专用）| 	无| 	否|
| volume| 	Boolean| 	音量开关，true为开启音量功能，false不开启（ios不支持音量功能）| 	无| 	否|
| fullscreenStart| 	方法| 	点击进入全屏回调函数（H5播放器专用）| 	无| 	否|
| fullscreenEnd| 	方法| 	点击退出全屏回调函数（H5播放器专用）| 	无| 	否|

### 播放器回调方法
| 参数 |	类型	| 说明|	返回值|	用法|
| :---: | :---: | :--- | :---: | :---: |
| turnOn |	方法 | ios开启弹幕	|无 |	_ejuInit.turnOn() |
| turnOdd |	方法 | ios关闭弹幕	|无 |	_ejuInit.turnOff() |
| messageAdd |	方法 | ios发送弹幕	|无 |	_ejuInit.messageAdd() |
| isCommentsOn |	方法 | ios返回弹幕是否开启	|布尔值 |	_ejuInit.isCommentsOn() |
| reload |	方法 | H5切换视频方法(H5播放器专用)	|无 |	_ejuInit.reload() |
