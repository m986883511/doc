# Python

## 爬虫

```en
import requests
print('访问baidu网站 获取Response对象')
headers = {'content-type': 'application/json',
            'User-Agent': r'Mozilla/5.0 (Linux; Android 9; NX609J Build/PKQ1.181021.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/66.0.3359.126 MQQBrowser/6.2 TBS/044904 Mobile Safari/537.36 MMWEBID/5292 MicroMessenger/7.0.6.1460(0x27000634) Process/tools NetType/WIFI Language/zh_CN',
           'Host':'dwmm136.cn',
           'Connection':'keep-alive',
           'Cache-Control: max-age':0,
           'Upgrade-Insecure-Requests': 1,
           'User-Agent': 'Mozilla/5.0 (Linux; Android 9; NX609J Build/PKQ1.181021.001; wv) AppleWebKit/537.36 (KHTML, like Gecko) Version/4.0 Chrome/66.0.3359.126 MQQBrowser/6.2 TBS/044904 Mobile Safari/537.36 MMWEBID/5292 MicroMessenger/7.0.6.1460(0x27000634) Process/tools NetType/WIFI Language/zh_CN',
           'Accept':'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,image/wxpic,image/sharpp,image/apng,image/tpg,*/*;q=0.8',
           'Referer':'http://dwmm136.cn/web/index.php?c=article&a=rtbus&do=line_ssgj&lineId=025-305%E8%B7%AF-0&lineNo=305%E8%B7%AF&name=305&direction=0',
           'Accept-Encoding':'gzip, deflate',
           'Accept-Language':'zh-CN,en-US;q=0.9',
           'Cookie': 'PHPSESSID=03u3cai9k953uvn34kt1gev847; Hm_lvt_416c770ac83a9d996d7b3793f8c4994d=1568547083; Hm_lpvt_416c770ac83a9d996d7b3793f8c4994d=1568557360'
           }

url = "http://dwmm136.cn/web/index.php?c=article&a=rtbus&do=line_ssgj&lineId=025-305%E8%B7%AF-0&lineNo=305%E8%B7%AF&name=305&direction=0 HTTP/1.1"
r = requests.get(url,headers)
print(r.status_code)
print(r.encoding)
print(r.apparent_encoding)
print('将对象编码转换成UTF-8编码并打印出来')
r.encoding = 'utf-8'
print(r.text)
```





```en
import hashlib
m1 = hashlib.md5()  # 使用md5对象里的update方法md5转换
```

[树莓派页面](raspberry.html)



