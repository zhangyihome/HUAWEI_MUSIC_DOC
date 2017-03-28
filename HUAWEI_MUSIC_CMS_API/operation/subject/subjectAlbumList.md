
#专题下专辑列表
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/subject/:subjectId/album/list/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|params|int|必须|专题ID|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|channelId|query|int|可选|频道ID|
|condition|query|string|可选|查询条件（albumId:专辑ID，albumName:专辑名称，albumNickName:别名，anchorName:主播，programName:默认播放节目）|
|key|query|string|可选|查询关键字|

## 响应
####响应成功
```
{
  "total": 2,
  "albums": [
    {
      "subjectAlbumId": 2,
      "subjectId": 1,
      "albumId": 2,
      "albumName": "胡泰然专辑2",
      "anchorName": "hutairan",
      "sortType": 15,
      "sort": 1,
      "adminId": 1,
      "createTime": "2017-03-22 11:19:56",
      "status": 1,
      "channelId": 51,
      "channelName": "音乐故事"
    },
    {
      "subjectAlbumId": 1,
      "subjectId": 1,
      "albumId": 1,
      "albumName": "胡泰然专辑1",
      "albumNickName": "新专辑",
      "anchorName": "hutairan",
      "sortType": 15,
      "sort": 2,
      "adminId": 1,
      "createTime": "2017-03-22 11:19:56",
      "status": 1,
      "channelId": 51,
      "channelName": "音乐故事"
    }
  ],
  "c": "s"
}
```
####未查询到数据
```
{
  "c": "f",
  "i": "没有找到符合条件的数据"
}
```