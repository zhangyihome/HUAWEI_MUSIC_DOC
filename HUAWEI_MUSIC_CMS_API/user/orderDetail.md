
# 频道下专辑列表
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|GET|/hmf/user/order/id/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|key|query|string|非必须|key可以是:albumId albumName hwId cuid orderId|
|value|query|string|非必须|查询条件：搜索关键值|
## 响应
```
{
  "order": {
    "id": 2,
    "orderId": "10001",
    "cuid": "123",
    "hwId": "132",
    "payType": 25,
    "albumId": 32,
    "albumName": "就回家了",
    "updateTime": "2017-03-24 11:20",
    "programNum": 9,
    "programIds": "12,13,14,15,16",
    "amount": 1,
    "tradeTime": "2017-03-02 15:52",
    "status": 1,
    "cTime": "2017-03-27 12:37"
  },
  "programList": [
    {
      "anchorName": "hutairan",
      "authorName": "asdf",
      "programId": 12,
      "albumId": 0,
      "anchorUserId": 0,
      "programName": "Various Artists - 苏维埃进行曲1",
      "albumName": "胡泰然专辑1",
      "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qe33r8.mp3",
      "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qe33r8.mp3",
      "format": "mp3",
      "fileSize": 6858712,
      "programSize": "6.5 MB",
      "duration": 167200,
      "bitRate": 320,
      "samplingRate": 44100,
      "convertStatus": 90,
      "sort": 0,
      "status": 0,
      "reviewStatus": 7,
      "reviewErrorId": 0,
      "adminId": 0,
      "durationFormat": "00:02:47"
    },
    {
      "anchorName": "hutairan",
      "authorName": "adf",
      "programId": 13,
      "albumId": 0,
      "anchorUserId": 0,
      "programName": "Finale - 九州缥缈录.乱世歌行",
      "albumName": "胡泰然专辑2",
      "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qdyxj7.mp3",
      "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qdyxj7.mp3",
      "format": "mp3",
      "fileSize": 3721669,
      "programSize": "3.5 MB",
      "duration": 145000,
      "bitRate": 192,
      "samplingRate": 44100,
      "convertStatus": 90,
      "sort": 0,
      "status": 0,
      "reviewStatus": 7,
      "reviewErrorId": 0,
      "adminId": 0,
      "durationFormat": "00:02:25"
    },
    {
      "anchorName": "hutairan",
      "authorName": "adf",
      "programId": 14,
      "albumId": 0,
      "anchorUserId": 0,
      "programName": "Various Artists - 苏维埃进行曲",
      "albumName": "胡泰然专辑2",
      "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qe33r8.mp3",
      "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qe33r8.mp3",
      "format": "mp3",
      "fileSize": 6858712,
      "programSize": "6.5 MB",
      "duration": 167200,
      "bitRate": 320,
      "samplingRate": 44100,
      "convertStatus": 90,
      "sort": 0,
      "status": 0,
      "reviewStatus": 7,
      "reviewErrorId": 0,
      "adminId": 0,
      "durationFormat": "00:02:47"
    },
    {
      "anchorName": "hutairan",
      "programId": 15,
      "albumId": 0,
      "anchorUserId": 0,
      "programName": "Finale - 九州缥缈录.乱世歌行",
      "albumName": "胡泰然专辑3",
      "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qdyxj7.mp3",
      "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qdyxj7.mp3",
      "format": "mp3",
      "fileSize": 3721669,
      "programSize": "3.5 MB",
      "duration": 145000,
      "bitRate": 192,
      "samplingRate": 44100,
      "convertStatus": 90,
      "sort": 0,
      "status": 0,
      "reviewStatus": 7,
      "reviewErrorId": 0,
      "adminId": 0,
      "durationFormat": "00:02:25"
    },
    {
      "anchorName": "hutairan",
      "programId": 16,
      "albumId": 0,
      "anchorUserId": 0,
      "programName": "Various Artists - 苏维埃进行曲",
      "albumName": "胡泰然专辑3",
      "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qe33r8.mp3",
      "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram10/audio/original/20170315/29qe33r8.mp3",
      "format": "mp3",
      "fileSize": 6858712,
      "programSize": "6.5 MB",
      "duration": 167200,
      "bitRate": 320,
      "samplingRate": 44100,
      "convertStatus": 90,
      "sort": 0,
      "status": 0,
      "reviewStatus": 7,
      "reviewErrorId": 0,
      "adminId": 0,
      "durationFormat": "00:02:47"
    }
  ],
  "c": "s"
}
```
