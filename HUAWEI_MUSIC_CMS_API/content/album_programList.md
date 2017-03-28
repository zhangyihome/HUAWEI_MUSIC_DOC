
# 同一专辑下的节目审核列表
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/album/：albumId/programs/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|reviewStatus|query|int|必须|审核状态:（7：待审核，8：审核通过，9：审核未通过）|
|convertStatus|query|int|必须|转码状态|
|key|query|String|非必须|关键词类型（id:节目ID、programName：节目名称）|
|value|query|string|非必须|查询条件：搜索关键词|
## 响应
```
{
  "list": [
    {
      "programId": 1, //节目ID
      "programName": "testProgram",//节目名称
      "updateTime": "2017-03-14 18:26", //更新时间
      "reviewStatus": 8, //审核状态
      "reviewTime": "2017-03-17 17:34", //审核时间
      "convertStatus": 0, //转码状态
      "sort":1 //序号
    }
  ],
  "total": 1,
  "c": "s"
}
```
