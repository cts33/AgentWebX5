

## AgentWebX5 介绍

基于腾讯X5内核版的 AgentWeb ，简单易用 ， 带有进度条 、 支持文件上传 、 下载 、 简化 Javascript 通信 、 链式调用  、性能更优 。更多使用请参照上面的 sample 。 

## AgentWeb 功能
1. 支持进度条以及自定义进度条
2. 支持文件下载
3. 支持文件下载断点续传
4. 支持下载通知形式提示进度
5. 简化 Javascript 通信 
6. 支持 Android 4.4 Kitkat 以及其他版本文件上传
7. 支持注入 Cookies
8. 支持全屏播放视频
9. Js 安全通信更简洁
10. 支持调起微信支付
11. 支持调起支付宝
12. 默认支持定位
13. 性能更优

## 引入

* Gradle 
   
   ```
   compile 'com.just.agentwebX5:agentwebX5:1.0.0'
   ```
* Maven
	
	```
	<dependency>
 	  <groupId>com.just.agentwebX5</groupId>
 	  <artifactId>agentwebX5</artifactId>
	  <version>1.0.0</version>
	  <type>pom</type>
	</dependency>
	
	```

## Android WebView
如果你更喜欢Android WebView ，请切换到这个仓库
[AgentWebX5](https://github.com/Justson/AgentWeb)

## 使用

1. 下载腾讯X5内核最新 SDK 导入项目中并依赖。
2. 引入 `AgentWebX5`
3. 需要全局初始化X5内核 `QbSdk.initX5Environment(getApplicationContext(),  cb);`


## 注意事项 
1. AgentWebX5 内部并没有直接依赖X5库 ，需要用户到[腾讯官网](https://x5.tencent.com/tbs/)下载 ， 并在项目中依赖该库 。
2. X5 内核的WebView ，由于不是 Google 官方控件， 所以很多第三方开源组件不支持 。
3. 支付宝需要引入[支付宝SDK](https://open.alipay.com/platform/home.htm)项目中依赖上支付宝SDK即可 ,微信支付不需要做任何操作。