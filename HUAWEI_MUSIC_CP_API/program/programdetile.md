# 节目详情
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/program/:programId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|programId|Params|int|必填|节目ID|




## 响应
```
{
  "programVO": {
    "programId": 88,
    "albumId": 24,
    "anchorUserId": 10,
    "programName": "F.I.R. - 你的微笑",
    "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5qmsb.mp3",
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5qmsb.mp3",
    "format": "mp3",
    "fileSize": 10825869,
    "duration": 261500,
    "bitRate": 320,
    "samplingRate": 44100,
    "sort": 1,
    "status": 1,
    "reviewStatus": 7,
    "createTime": "2017-03-22 13:23:38.0",
    "node": "node1"
  },
  "c": "s"
}
```


