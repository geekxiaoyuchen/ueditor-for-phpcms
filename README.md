# ueditor-for-phpcms

# 简介
Phpcms是国内一款免费开源的CMS，使用者众多，但是近年来更新和维护基本处于停止状态。最为大家所诟病的是自带的编辑是很老版本的CKeditor，基本上不能满足一般网站的需求。特别是商业客户的需求。

为了解决这个问题，很多朋友考虑将编辑器更换成百度的Ueditor，但是在更改的过程中都不同程度的遇到了问题。本人经过测试，实现了完美的集成，分享代码。

# 使用

1、直接下载源码到phpcms根目录；

2、修改ueditor配置文件，/statics/js/ueditor/php/config.json;
```php
{
  "imageActionName": "uploadimage",
  "imageFieldName": "upfile",
  "imageMaxSize": 2048000,
  "imageAllowFiles": [".png",".jpg",".jpeg",".gif",".bmp",".*"],
  "imageCompressEnable": true,
  "imageCompressBorder": 1600,
  "imageInsertAlign": "none",
  "imageUrlPrefix": "",
  "imagePathFormat": "/jingxiao/uploadfile/{yyyy}/{mm}{dd}/{yyyy}{mm}{dd}{rand:6}",
  "scrawlActionName": "uploadscrawl",
  "scrawlFieldName": "upfile",
  "scrawlPathFormat": "/jingxiao/uploadfile/{yyyy}/{mm}{dd}/{time}{rand:6}",
  "scrawlMaxSize": 20480000,
  "scrawlUrlPrefix": "",
  "scrawlInsertAlign": "none",
  "snapscreenActionName": "uploadimage",
  "snapscreenPathFormat": "/jingxiao/uploadfile/{yyyy}/{mm}{dd}/{time}{rand:6}",
  "snapscreenUrlPrefix": "",
  "snapscreenInsertAlign": "none",
  "catcherLocalDomain": ["127.0.0.1", "localhost", "img.baidu.com"],
  "catcherActionName": "catchimage",
  "catcherFieldName": "source",
  "catcherPathFormat": "/jingxiao/uploadfile/{yyyy}/{mm}{dd}/{time}{rand:6}",
  "catcherUrlPrefix": "",
  "catcherMaxSize": 2048000,
  "catcherAllowFiles": [".png", ".jpg", ".jpeg", ".gif", ".bmp"],
  "videoActionName": "uploadvideo",
  "videoFieldName": "upfile",
  "videoPathFormat": "/jingxiao/uploadfile/{yyyy}/{mm}{dd}/{yyyy}{mm}{dd}{rand:6}",
  "videoUrlPrefix": "",
  "videoMaxSize": 102400000,
  "videoAllowFiles": [
    ".flv", ".swf", ".mkv", ".avi", ".rm", ".rmvb", ".mpeg", ".mpg",
    ".ogg", ".ogv", ".mov", ".wmv", ".mp4", ".webm", ".mp3", ".wav", ".mid"],
  "fileActionName": "uploadfile",
  "fileFieldName": "upfile",
  "filePathFormat": "/jingxiao/uploadfile/{yyyy}/{mm}{dd}/{yyyy}{mm}{dd}{rand:6}",
  "fileUrlPrefix": "",
  "fileMaxSize": 51200000,
  "fileAllowFiles": [
    ".png", ".jpg", ".jpeg", ".gif", ".bmp",
    ".flv", ".swf", ".mkv", ".avi", ".rm", ".rmvb", ".mpeg", ".mpg",
    ".ogg", ".ogv", ".mov", ".wmv", ".mp4", ".webm", ".mp3", ".wav", ".mid",
    ".rar", ".zip", ".tar", ".gz", ".7z", ".bz2", ".cab", ".iso",
    ".doc", ".docx", ".xls", ".xlsx", ".ppt", ".pptx", ".pdf", ".txt", ".md", ".xml"
  ],
  "imageManagerActionName": "listimage",
  "imageManagerListPath": "/jingxiao/uploadfile/",
  "imageManagerListSize": 20,
  "imageManagerUrlPrefix": "",
  "imageManagerInsertAlign": "none",
  "imageManagerAllowFiles": [".png", ".jpg", ".jpeg", ".gif", ".bmp"],
  "fileManagerActionName": "listfile",
  "fileManagerListPath": "/jingxiao/uploadfile/",
  "fileManagerUrlPrefix": "",
  "fileManagerListSize": 20,
  "fileManagerAllowFiles": [
    ".png", ".jpg", ".jpeg", ".gif", ".bmp",
    ".flv", ".swf", ".mkv", ".avi", ".rm", ".rmvb", ".mpeg", ".mpg",
    ".ogg", ".ogv", ".mov", ".wmv", ".mp4", ".webm", ".mp3", ".wav", ".mid",
    ".rar", ".zip", ".tar", ".gz", ".7z", ".bz2", ".cab", ".iso",
    ".doc", ".docx", ".xls", ".xlsx", ".ppt", ".pptx", ".pdf", ".txt", ".md", ".xml"
  ]
}
```

根据网站目录的实际情况修改上传路径，特别提醒，这个文件中千万不要加注释！

# 后记

如果在使用中遇到任何问题，欢迎加萧队长微信共同探讨！（微信号：geekxiaoyuchen）

Happy Hacking :)




