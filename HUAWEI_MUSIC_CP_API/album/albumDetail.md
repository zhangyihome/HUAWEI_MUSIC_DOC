#专辑详情
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/album/:albumId|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|
## 响应
####响应成功
```
{
  "albumVO": {
    "albumId": 5,
    "anchorUserId": 10,
    "albumName": "胡泰然专辑5",
    "albumType": 12,
    "albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/cover/album/20170316/29sbt9e1.png",
    "channelId": 51,
    "anchorName": "hutairan",
    "updateStatus": 21,
    "updateTime": "2017-03-16 13:46:38.0",
    "tags": "1,2,3",
    "summary": "假数据",
    "copyrightUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg,http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg",
    "agreementUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/agreement/20170316/29sfj1xp.jpg",
    "status": 1,
    "reviewStatus": 7,
    "createTime": "2017-03-16 13:46:38.0",
    "copyrightUrlList": [
      "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg",
      "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg"
    ],
    "tagsList": [
      {
        "tagId": 1,
        "tagName": "tag1",
        "channelId": 59
      },
      {
        "tagId": 2,
        "tagName": "tag2",
        "channelId": 59
      },
      {
        "tagId": 3,
        "tagName": "tag3",
        "channelId": 59
      }
    ]
  },
  "c": "s"
}
```
####响应失败
```
{
  "c": "f",
  "i": "没有找到符合条件的数据"
}
```