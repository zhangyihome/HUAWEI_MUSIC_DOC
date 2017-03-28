
#标签列表
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/tag/list/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|channelId|query|int|可选|频道ID|

## 响应
####响应成功
```
{
  "total": 5,
  "hmfTags": [
    {
      "tagId": 2,
      "tagName": "testTag",
      "channelId": 59,
      "adminId": 0,
      "status": 1
    },
    {
      "tagId": 3,
      "tagName": "tag3",
      "channelId": 59,
      "adminId": 0,
      "status": 1
    },
    {
      "tagId": 4,
      "tagName": "新的标签",
      "channelId": 63,
      "adminId": 0,
      "status": 1
    },
    {
      "tagId": 5,
      "tagName": "tag5",
      "channelId": 62,
      "adminId": 0,
      "status": 1
    },
    {
      "tagId": 6,
      "tagName": "新建标签",
      "channelId": 65,
      "adminId": 15,
      "createTime": "2017-03-17 10:52:20",
      "status": 1
    }
  ],
  "c": "s"
}
```
####未查询到数据
```
{
  "c": "f",
  "i": "数据为空"
}
```