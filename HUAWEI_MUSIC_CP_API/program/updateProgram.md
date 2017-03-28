# 修改节目
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|PUT|/amp/program/:programId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|programId|Params|int|必填|节目ID|
|programName|Body|String|必填|节目名称|
|webUrl|Body|String|必填|web路径|
|filePath|Body|String|必填|服务器路径 |
|format|Body|String|必填|音频类型|
|fileSize|Body|long|必填|文件大小|
|duration|Body|long|必填|时长|
|bitRate|Body|int|必填|比特率|
|samplingRate|Body|int|必填|采样率|
|audio|Body|AudioInfoVO|非必填|音频信息（参见表audio）|
|file|Body|FileVO|非必填|文件信息（参见表file）|
|node|Body|String|必填|上传节点|

##表audio
|名称|位置|类型|约束|描述|
|--|--|--|--|
|duration|Body|Long|必填|音频时长|
|bitRate|Body|int|必填|音频比特率|
|channels|Body|int|必填|音频通道|
|samplingRate|Body|int|必填|采样频率|

##表file
|名称|位置|类型|约束|描述|
|--|--|--|--|
|fileOrigName|Body|String|必填|音频源名字|
|filePath|Body|String|必填|音频路径|
|fileSize|Body|Long|必填|音频文件大小|
|webUrl|Body|String|必填|音频地址|

##参数说明
若重新上传音频文件 则需要上传audio和file  会覆盖原来的数据
若不重新上传音频 则programName以下必填信息会在之前请求接口中获取
新添加参数node 若为新上传的音频则在上传音频接口的返回值中获取node，否则是原数据中的node

##添加数据json格式
```
{

    "albumId": 1,
    "anchorUserId": 1,
    "programName": "A-Lin - 给我一个理由忘记12346",
    "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram1/audio/original/20170314/29mw2dew.mp3",
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram1/audio/original/20170314/29mw2dew.mp3",
    "format": "mp3",
    "fileSize": 12430732,
    "duration": 283600,
    "bitRate": 320,
    "samplingRate": 44100,
    "sort": 5,
    "status": 1,
    "reviewStatus": 7,
    "createTime": "2017-03-15 14:56:03.0",
    "file": {
		"filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5dtf6.mp3",
		"webUrl": "http://192.168.2.206/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5dtf6.mp3",
		"fileNewName": "2aa5dtf6.mp3",
		"fileOrigName": "G.E.M.邓紫棋 - 喜欢你.mp3",
		"fileSize": 9920472
	},
	"audio": {
		"duration": 239000,
		"bitRate": 320,
		"samplingRate": 44100,
		"format": "mp3",
		"channels": 2
	},
	"node": "node2"
}
```
  
## 响应
####响应成功
```json
{
  "c": "s"
}
```

#### 参数错误
```json
{
  "c": "f",
  "i": "参数错误"
}
```


