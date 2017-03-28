
# 专辑详情
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/program/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|节目ID|
## 响应
```
{
  "program": {
    "anchorName": "hutairan",	//主播名称
    "authorName": "asdf",	//作者名称
    "programId": 1,	//节目id
    "albumId": 0,	//专辑id
    "anchorUserId": 0,	//主播id
    "programName": "testProgram",	//节目名称
    "albumName": "胡泰然专辑1",	//专辑名称
    "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram1/audio/original/20170314/29mw2dew.mp3",
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram1/audio/original/20170314/29mw2dew.mp3",
    "format": "mp3",	//文件格式
    "fileSize": 12430732,	//节目大小
    "programSize": "11.9 MB",	//节目大小
    "duration": 283600,	//时长
    "bitRate": 320,	//码率
    "samplingRate": 44100,	//采样率
    "convertStatus": 90,	//转码状态
    "sort": 0,	//排序序号
    "status": 0,	//是否可用
    "reviewStatus": 8,	//审核状态
    "reviewErrorId": 0,	//审核不通过原因
    "adminId": 0,	//后台用户id
    "durationFormat": "00:04:43"	//时长
  },
  "c": "s"
}
```
