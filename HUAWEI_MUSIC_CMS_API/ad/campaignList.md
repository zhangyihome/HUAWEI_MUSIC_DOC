
# 广告投放列表
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/ad/info/campaigns/:pageNo/:pageSize|

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
      "scheduleStart": "2017-03-20", // 排期开始时间
      "scheduleEnd": "2017-04-20", // 排期结束时间
      "status": 154, // 状态【153：暂停，154：执行】
      "weight": 5, // 权重
      "runStatus": 156, // 执行状态【156：等待投放，157：投放中，158：投放结束】
      "campaignName": "华为守机", // 广告名称
      "campaignId": 6 // 广告ID
    },
    {
      "scheduleStart": "2016-12-12",
      "scheduleEnd": "2017-06-06",
      "status": 154,
      "weight": 5,
      "runStatus": 157,
      "campaignName": "更新测试",
      "campaignId": 4
    }
  ],
  "total": 2,
  "c": "s"
}
```
