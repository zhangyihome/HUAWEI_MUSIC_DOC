
# 广告数据的详细信息
<font color="gray" size="3">@author：张毅</font>

|METHOD|URI|  
|--|--|  
|GET|/hmf/ad/stat/:campaignId/details/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|  
|--|--|--|--|  
|campaignId|params|int|必须|广告活动id  
|pageNo|params|int|必须|当前页码|  
|pageSize|params|int|必须|每页数据数目|  
|startTime|query|String|非必须|查询条件：投放开始时间|  
|endTime|query|String|非必须|查询条件：投放结束时间|  

## 响应
```
{
    "list": [
        {
            "id": 3, //明细数据ID
            "campaignId": 4, //广告活动ID
            "dayTime": "2017-03-15", //统计日期
            "playNum": 9, //广告展示量
            "clickNum": 6, //广告点击量
            "cRate": 66.66666666666667, //广告点击率
            "distinctPlayNum": 5, //独立展示量
            "distinctClickNum": 5 //独立点击量
        },
        {
            "id": 4,
            "campaignId": 4,
            "dayTime": "2017-03-15",
            "playNum": 4,
            "clickNum": 5,
            "cRate": 125,
            "distinctPlayNum": 5,
            "distinctClickNum": 7
        }
    ],
    "sumVo": {
      "campaignName": "更新测试", //广告活动名称
      "scheduleStart": "2016-12-12", //投放开始时间
      "scheduleEnd": "2017-06-06", //投放结束时间
      "status": 153, // 广告状态
      "playNum": 13, // 总广告展示量
      "clickNum": 11, // 总广告点击量
      "cRate": 84.62, // 总广告点击率
      "distinctPlayNum": 10, // 总独立展示量
      "distinctClickNum": 12 // 总独立点击量
    },
    "total": 2,
    "c": "s"
}
```