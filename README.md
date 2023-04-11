# 食用方法

此程序基于ThinkPHP5.1 PHP版本需`7.0-7.4`之间。

`Nginx`请设置如下`伪静态` `Apache`无需配置 运行目录`默认`即可
```
location / {
	if (!-e $request_filename){
		rewrite  ^(.*)$  /index.php?s=$1  last;   break;
	}
}
```

将程序上传至网站根目录,访问`域名/install`进行安装操作



# 免责声明

本仓库只为学习研究，如涉及侵犯个人或者团体利益，请与我取得联系，我将主动删除一切相关资料，谢谢！
