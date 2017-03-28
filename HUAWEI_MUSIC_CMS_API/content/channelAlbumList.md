
# 运营管理添加专辑查询接口
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/album/list/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|key|query|String|非必须|关键词类型（albumId:专辑ID、albumName：专辑名|
|value|query|string|非必须|查询条件：搜索关键词|
## 响应
```
{
  "list": [
    {
      "albumId": 1,
      "albumName": "胡泰然专辑1",
      "albumType": 0,
      "anchorName": "hutairan",
      "price": 0
    },
    {
      "albumId": 2,
      "albumName": "胡泰然专辑2",
      "albumType": 0,
      "anchorName": "hutairan",
      "price": 0
    },
    {
      "albumId": 4,
      "albumName": "胡泰然专辑4",
      "albumType": 0,
      "anchorName": "hutairan",
      "price": 0
    },
    {
      "albumId": 5,
      "albumName": "胡泰然专辑5",
      "albumType": 0,
      "anchorName": "hutairan",
      "price": 0
    }
  ],
  "total": 4,
  "c": "s"
}
```
