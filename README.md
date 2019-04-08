# jwc_news.yangtzeu
长江大学教务处新闻通知api接口


**简要描述：**

- 长江大学教务处新闻通知接口

**请求URL：**
- ` http://app.dreamfish.online/news `

**请求方式：**
- GET

**参数：**

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|kind |是  |string |新闻类型（jwtz、bzsw、jxdt、jxjb、gjxx）  |
|page |是  |int | 页数 (需大于零)   |

 **返回示例**

```
{
  "msg": "success",
  "code": 200,
  "data": {
    "kind": "教务通知",
    "all_page": 137,
    "now_page": 1,
    "news": [
      {
        "title": "2018-2019学年第二学期荆州校区国学大讲堂开班通知",
        "date": "2019-04-08",
        "kind": "教务通知",
        "content_url": "http://jwc.yangtzeu.edu.cn/../info/1083/5903.htm"
      },
      {
        "title": "长江大学关于公布三百名师计划2018年度教学名师的通知",
        "date": "2019-03-11",
        "kind": "教务通知",
        "content_url": "http://jwc.yangtzeu.edu.cn/../info/1083/5844.htm"
      }
    ]
  }
}
```

 **返回参数说明**

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|msg |string   |请求结果，success：成功；failure：失败  |
|code |int   |请求结果码，200：成功；400：失败  |
|data |$data   |响应数据，$data：数据集；null：失败  |
|kind |string   |新闻通知类型：教务通知、本周事务、教学动态、教学简报、高教信息  |
|all_page |int   |请求的新闻通知栏目总页数  |
|now_page |int   |当前请求新闻通知的页数  |
|news |list<$news>   |当前请求新闻通知结果集  |
|title |string   |新闻通知标题  |
|date |string   |新闻通知发布时间  |
|content_url |string   |新闻通知详情链接  |

 **备注**

- 若接口失效请联系，QQ：[1223414335](http://qm.qq.com/cgi-bin/qm/qr?k=z2XFXTzDNSwr-kfZ9lC2FafXsfYhVTJa "1223414335")
- 欢迎加入我们，QQ群：[617082514](http://qm.qq.com/cgi-bin/qm/qr?k=zkeHz0NMV_dwdhJxSLCaqPSbzsbnXmiz "617082514")
