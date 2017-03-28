
# 广告活动详情
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/ad/info/campaigns/：id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|广告活动ID|
## 响应
####响应成功
```
{
  "campaign": {
    "position": 151, // 广告位置
    "scheduleStart": "2016-12-12", // 排期开始时间
    "scheduleEnd": "2017-03-15", // 排期结束时间
    "status": 154, // 广告状态
    "weight": 5, // 广告权重
    "url": "www.baidu.com", // 链接地址
    "scheme": "文案内容...", // 广告文案
    "creativeUrl": "www.goole.com", // 素材地址
    "scheduleList": [ // 排期明细
      "2016-12-12",
      "2016-12-22",
      "2016-12-23",
      "2016-12-24",
      "2017-03-15"
    ],
    "campaignName": "你好", // 广告活动名称
    "campaignId": 1 // 广告活动ID
  },
  "c": "s"
}
```
####响应失败
```
{
    "c":"f",
    "i":"参数错误！"
}
```