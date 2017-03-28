
# 频道下专辑列表
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/channel/album/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|channelId|query|int|非必须|查询条件：频道Id|
|updateStatus|query|int|非必须|更新状态:21更新中 22完结|
|priceType|query|int|非必须|定价类型:23免费  24专辑  25多集|
|onlineStatus|query|int|非必须|上线状态:18未上架  19已上架  20已下架|
|isRecommend|query|int|非必须|查询条件：是否推荐  15正常 16推荐|
|key|query|string|非必须|key可以是:albumId albumName programName albumNickName anchorName|
|value|query|string|非必须|查询条件：搜索关键值|
## 响应
```
{
  "list" : [ {
      "albumId": 1,	//专辑id
      "anchorUserId": 10,	//主播id
      "albumName": "胡泰然专辑1",	//专辑名称
      "albumType": 12,	//专辑类型
      "albumNickName": "测",	//专辑昵称
      "channelId": 51,	//频道id
      "anchorName": "hutairan",	//主播名称
      "updateStatus": 21,	//更新状态(更新中,已完结)
      "updateTime": "2017-03-22 13:20",	//最后更新时间
      "reviewStatus": 8,	//审核状态
      "reviewTime": "2017-03-22 17:28:51.0",	//审核时间
      "audition": 10,	//试听数量
      "playProgramId": 1,	//默认播放id
      "isRecommend": 15,	//是否推荐  15正常  16推荐
      "onlineStatus": 19,	//上架状态
      "onlineTime": "2017-03-22 17:29:04.0",	//上架时间
      "offlineTime": "2017-03-22 17:29:09.0",	//下架时间
      "priceType": 24,	//定价类型23免费 24专辑  25多集
      "price": 1,	//价钱
      "sort": 1,	//序号
      "sortType": 26,	//排序类型26正序  27倒序
      "createTime": "2017-03-15 18:37",	//创建时间
      "programNum": 13	//节目数量
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
