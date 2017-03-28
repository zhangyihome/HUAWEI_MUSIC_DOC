
#举报列表
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/alarm/list/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|status|query|int|可选|处理状态(5:未处理， 6：已处理)|
|channelId|query|int|可选|频道ID|
|reasonId|query|int|可选|举报理由ID(100:无法播放，无故暂停， 101:节目含有欺诈、反动、色情内容， 102:章节不完整，集数排序错误， 103:音质太差)|
|condition|query|string|可选|查询条件（id:ID,program:节目名称,album:专辑名称）|
|key|query|string|可选|查询关键字|

## 响应
####响应成功
```
{
  "total": 3,
  "hmfAlarms": [
    {
      "alarmId": 3,
      "programId": 1,
      "programName": "testProgram",
      "albumId": 2,
      "albumName": "胡泰然专辑2",
      "channelId": 66,
      "channelName": "人文社科",
      "userId": 4,
      "resonId": 103,
      "reason": "音质太差",
      "createTime": "2017-03-15 11:25:18",
      "status": 6,
      "statusInfo": "已处理"
    },
    {
      "alarmId": 2,
      "programId": 2,
      "programName": "A-Lin - 给我一个理由忘记",
      "albumId": 2,
      "albumName": "胡泰然专辑2",
      "channelId": 59,
      "channelName": "惊悚悬疑",
      "userId": 2,
      "resonId": 101,
      "reason": "节目含有欺诈、反动、色情内容",
      "createTime": "2017-03-14 16:04:37",
      "status": 6,
      "statusInfo": "已处理"
    },
    {
      "alarmId": 1,
      "programId": 1,
      "programName": "testProgram",
      "albumId": 1,
      "albumName": "胡泰然专辑1",
      "channelId": 51,
      "channelName": "音乐故事",
      "userId": 1,
      "resonId": 100,
      "reason": "无法播放，无故暂停",
      "createTime": "2017-03-13 17:28:51",
      "status": 6,
      "statusInfo": "已处理"
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