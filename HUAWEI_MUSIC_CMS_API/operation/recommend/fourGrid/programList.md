
# 专辑下节目列表
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/recommend/fourGrid/:position/:albumId/programs/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|position|params|int|必须|四宫格位置1,2,3,4|
|albumId|params|int|必须|专辑id|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|key|query|string|非必须|key可以是:id:节目id programName:节目名称|
|value|query|string|非必须|查询条件：搜索关键值|
## 响应
```
{
  "list": [
    {
      "programId": 1, //节目ID
      "programName": "testProgram",//节目名称
       "albumName": "胡泰然专辑1", //专辑名
      "anchorName": "hutairan", //主播名
      "updateTime": "2017-03-14 18:26", //更新时间
      "reviewStatus": 8, //审核状态
      "reviewTime": "2017-03-17 17:34", //审核时间
      "convertStatus": 0, //转码状态
      "channelId": 51,// 频道ID
      "sort":1 //序号
    }
  ],
  "total": 1,
  "c": "s"
}
```
