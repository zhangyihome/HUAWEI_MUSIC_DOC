
#专题下所有专辑
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/subject/:subjectId/album/list|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|params|int|必须|专题ID|

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
      "sortType": 15,
      "sort": 1,
      "adminId": 1,
      "createTime": "2017-03-22 11:19:56",
      "status": 1
    },
    {
      "subjectAlbumId": 1,
      "subjectId": 1,
      "albumId": 1,
      "albumName": "胡泰然专辑1",
      "albumNickName": "新专辑",
      "sortType": 15,
      "sort": 2,
      "adminId": 1,
      "createTime": "2017-03-22 11:19:56",
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
  "i": "没有找到符合条件的数据"
}
```