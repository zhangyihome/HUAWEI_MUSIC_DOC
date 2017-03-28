# 节目列表
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/album/:albumId/program/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|Params|int|必填|专辑ID|
|pageNo|Params|int|必填|页号|
|pageSize|Params|int|必填|每页多少条|
|keyword|Query|String|选填|条件|
|reviewStatus|Query|String|选填|审核状态|

## 响应
####响应成功
```json
{
  "pagelist": [
    {
      "programId": 21,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "Beyond - 情人1",
      "format": "12.1 MB",
      "fileSize": 12738357,
      "duration": 317000,
      "sort": 13,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:05:17"
    },
    {
      "programId": 12,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "Various Artists - 苏维埃进行曲1",
      "format": "6.5 MB",
      "fileSize": 6858712,
      "duration": 167200,
      "sort": 12,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:02:47"
    },
    {
      "programId": 11,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "Finale - 九州缥缈录.乱世歌行1",
      "format": "3.5 MB",
      "fileSize": 3721669,
      "duration": 145000,
      "sort": 11,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:02:25"
    },
    {
      "programId": 10,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "F.I.R. - 月牙湾",
      "format": "12.3 MB",
      "fileSize": 12879852,
      "duration": 308500,
      "sort": 10,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:05:08"
    },
    {
      "programId": 9,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "Beyond - 情人",
      "format": "12.1 MB",
      "fileSize": 12738357,
      "duration": 317000,
      "sort": 9,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:05:17"
    },
    {
      "programId": 8,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "Various Artists - 苏维埃进行曲",
      "format": "6.5 MB",
      "fileSize": 6858712,
      "duration": 167200,
      "sort": 8,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:02:47"
    },
    {
      "programId": 7,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "Finale - 九州缥缈录.乱世歌行",
      "format": "3.5 MB",
      "fileSize": 3721669,
      "duration": 145000,
      "sort": 7,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:02:25"
    },
    {
      "programId": 6,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "A-Lin - 给我一个理由忘记12346",
      "format": "12.7 MB",
      "fileSize": 13363612,
      "duration": 326000,
      "sort": 6,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:05:26"
    },
    {
      "programId": 5,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "A-Lin - 给我一个理由忘记1234",
      "format": "12.7 MB",
      "fileSize": 13363612,
      "duration": 326000,
      "sort": 5,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:05:26"
    },
    {
      "programId": 4,
      "albumId": 1,
      "anchorUserId": 10,
      "programName": "A-Lin - 给我一个理由忘记12",
      "format": "11.9 MB",
      "fileSize": 12430732,
      "duration": 283600,
      "sort": 4,
      "status": 0,
      "reviewStatus": 7,
      "durationTime": "00:04:43"
    }
  ],
  "total": 12,
  "c": "s"
}
```



