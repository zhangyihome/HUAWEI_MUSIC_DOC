# 节目音频上传
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|POST|/amp/program/audio|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|uploadFile|Body|MultipartFile|必填|上传的音频|

## 示例

## 响应
```
{
  "fileVO": {
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5sey4.mp3",
    "webUrl": "http://192.168.2.206/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5sey4.mp3",
    "fileNewName": "2aa5sey4.mp3",
    "fileOrigName": "F.I.R. - 月牙湾.mp3",
    "fileSize": 12879852
  },
  "audioInfoVO": {
    "duration": 308500,
    "bitRate": 320,
    "samplingRate": 44100,
    "format": "mp3",
    "channels": 2
  },
  "node": "node2",
  "c": "s"
}
```


