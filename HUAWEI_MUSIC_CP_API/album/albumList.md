
#专辑列表
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/album/list/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|keyword|query|string|可选|专辑名字|
|reviewStatus|query|int|可选|专辑状态（7：待审核，8：已通过，9：未通过）|

## 响应
```
{
  "pagelist": [
    {
      "albumId": 4,
      "anchorUserId": 10,
      "albumName": "胡泰然专辑4",
      "albumType": 12,
      "albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/cover/album/20170316/29sbt9e1.png",
      "channelId": 51,
      "anchorName": "hutairan",
      "updateStatus": 11,
      "updateTime": "2017-03-16 11:05:46.0",
      "tags": "1,2,3",
      "summary": "假数据",
      "agreementUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/agreement/20170316/29sfj1xp.jpg",
      "status": 1,
      "reviewStatus": 7,
      "createTime": "2017-03-16 11:05:46.0"
    },
    {
      "albumId": 2,
      "anchorUserId": 10,
      "albumName": "胡泰然专辑2",
      "albumType": 12,
      "albumCover": "fengmiangtest",
      "channelId": 51,
      "anchorName": "hutairan",
      "updateStatus": 11,
      "updateTime": "2017-03-16 09:54:20.0",
      "tags": "1,2,3",
      "summary": "假数据",
      "agreementUrl": "123231231232",
      "status": 1,
      "reviewStatus": 9,
      "createTime": "2017-03-16 09:54:20.0"
    },
    {
      "albumId": 1,
      "anchorUserId": 10,
      "albumName": "胡泰然专辑1",
      "albumType": 12,
      "channelId": 51,
      "anchorName": "hutairan",
      "updateStatus": 11,
      "updateTime": "2017-03-15 18:37:50.0",
      "tags": "1,2,3",
      "summary": "假数据",
      "agreementUrl": "123231231232",
      "status": 1,
      "reviewStatus": 7,
      "createTime": "2017-03-15 18:37:50.0"
    }
  ],
  "total": 3,
  "c": "s"
}
```