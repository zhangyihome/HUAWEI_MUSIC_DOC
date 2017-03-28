
# 广告数据列表
<font color="gray" size="3">@author：张毅</font>

|METHOD|URI|  
|--|--|  
|GET|/hmf/ad/stat/:pageNo/:pageSize|  

## 参数

|名称|位置|类型|约束|描述|  
|--|--|--|--|  
|pageNo|params|int|必须|当前页码|  
|pageSize|params|int|必须|每页数据数目|  
|startTime|query|String|非必须|查询条件：投放开始时间|  
|endTime|query|String|非必须|查询条件：投放结束时间|  
|campaignName|query|string|非必须|查询条件：搜索关键词|
## 响应
```
{
    "list": [
        {
            "campaignId": 1, //广告活动ID
            "campaignName": "你好", //广告活动名称
            "scheduleStart": "2016-12-12", //投放开始时间
            "scheduleEnd": "2017-03-15", //投放结束时间
            "playNum": 2, //广告展示量
            "clickNum": 1, //广告点击量
            "cRate": 50 //广告点击率
        },
        {
            "campaignId": 4,
            "campaignName": "更新测试",
            "scheduleStart": "2016-12-12",
            "scheduleEnd": "2017-06-06",
            "playNum": 13,
            "clickNum": 11,
            "cRate": 84.61538461538461
        },
        {
            "campaignId": 5,
            "campaignName": "更新测试",
            "scheduleStart": "2016-12-12",
            "scheduleEnd": "2017-01-01",
            "playNum": 0,
            "clickNum": 0,
            "cRate": 0
        }
    ],
    "total": 3,
    "c": "s"
}
```