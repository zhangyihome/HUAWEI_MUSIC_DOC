
# 电台排行榜列表
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/recommend/rank/findPage/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|channelId|query|int|非必须|查询条件：频道Id|
|isRecommend|query|boolean|非必须|查询条件：是否推荐|
|key|query|string|非必须|key可以是:albumId albumName programName albumNickName anchorName|
|value|query|string|非必须|查询条件：搜索关键值|
## 响应
```
{
  "listenList" : [ {
    "albumId" : 5,
    "albumName" : "胡泰然专辑5",
    "albumNickName" : "sdf",				//昵称
    "sortType" : 6,							//正常=15, 推荐=16
    "sort" : 7,
    "anchorName" : "hutairan",
    "channelId" : 51,						//频道Id
    "createTime" : "2017-03-18 15:51:44.0",
    "status" : 1
  }, {
    "albumId" : 1,
    "albumName" : "胡泰然专辑1",
    "albumNickName" : "sdf",
    "sortType" : 7,
    "sort" : 6,
    "defaultProgramId" : 1,
    "programName" : "testProgram",
    "anchorName" : "hutairan",
    "channelId" : 51,
    "createTime" : "2017-03-18 15:43:29.0",
    "status" : 1
  }, {
    "albumId" : 4,
    "albumName" : "胡泰然专辑4",
    "albumNickName" : "fgh",
    "sortType" : 7,
    "sort" : 5,
    "defaultProgramId" : 1,
    "programName" : "testProgram",
    "anchorName" : "hutairan",
    "channelId" : 51,
    "createTime" : "2017-03-18 15:39:39.0",
    "status" : 1
  }, {
    "albumId" : 6,
    "albumName" : "胡泰然专辑6",
    "albumNickName" : "sdf",
    "sortType" : 6,
    "sort" : 4,
    "anchorName" : "hutairan",
    "channelId" : 51,
    "createTime" : "2017-03-18 15:53:55.0",
    "status" : 1
  }, {
    "albumId" : 3,
    "albumName" : "胡泰然专辑3",
    "albumNickName" : "123",
    "sortType" : 7,
    "sort" : 3,
    "defaultProgramId" : 1,
    "programName" : "testProgram",
    "anchorName" : "hutairan",
    "channelId" : 51,
    "createTime" : "2017-03-18 15:20:41.0",
    "status" : 1
  }, {
    "albumId" : 7,
    "albumName" : "胡泰然专辑7",
    "albumNickName" : "sdf",
    "sortType" : 6,
    "sort" : 2,
    "anchorName" : "hutairan",
    "channelId" : 59,
    "createTime" : "2017-03-18 15:55:50.0",
    "status" : 1
  }, {
    "albumId" : 2,
    "albumName" : "胡泰然专辑2",
    "albumNickName" : "rty",
    "sortType" : 6,
    "sort" : 1,
    "defaultProgramId" : 1,
    "programName" : "testProgram",
    "anchorName" : "hutairan",
    "channelId" : 51,
    "createTime" : "2017-03-18 15:20:18.0",
    "status" : 1
  } ],
  "total" : 7,
  "c" : "s"
}
```
