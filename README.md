# CRAWL_WEB： 本工具主要功能为爬取太平洋电脑网中所有手机详细信息的地址



## 网页爬取规则：

1. 网页首页 URL 是 http://product.pconline.com.cn/mobile/0s1.shtml
2. 如果页面中可以点击下一页按钮，则下一页地址为 http://product.pconline.com.cn/mobile/25s1.shtml
**其中：0s1.shtml 变为25s1.shtml ，自增25**

找出网页规律后，开始爬取页面中的 URL 地址，将所有地址写入 txt 文件中，后续将继续爬取手机详细信息



## 以下为日志中打印的部分信息

```
[2018-01-05 23:01:16] INFO crawl_web.py[line:22] 开始处理 http://product.pconline.com.cn/mobile/0s1.shtml 网页数据:
[2018-01-05 23:02:22] INFO crawl_web.py[line:44]  检测到 23 个手机网址，写入文件成功
[2018-01-05 23:02:22] INFO crawl_web.py[line:95] 总共爬取 2948 个手机信
```

<u>总共爬取2948个手机地址，与网站中手机信息总数一致；脚本执行总耗时66秒，平均一秒爬取44个</u>





