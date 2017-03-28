# 添加单个节目
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|POST|/amp/album/:albumId/program/single|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必填|专辑ID|
|programName|Body|String|必填|节目名称|
|audio|Body|AudioInfoVO|必填|音频信息（参见表audio）|
|file|Body|FileVO|必填|文件信息（参见表file）|
|node|Body|String|必填|上传节点|

##表audio

|名称|位置|类型|约束|描述|
|--|--|--|--|
|duration|Body|Long|必填|音频时长|
|bitRate|Body|int|必填|音频比特率|
|channels|Body|int|必填|音频通道|
|samplingRate|Body|int|必填|采样频率|
|format|Body|String|必填|音频格式|

##表file

|名称|位置|类型|约束|描述|
|--|--|--|--|
|fileOrigName|Body|String|必填|音频源名字|
|fileNewName|Body|String|非必填|音频新名字|
|filePath|Body|String|必填|音频路径|
|fileSize|Body|Long|必填|音频文件大小|
|webUrl|Body|String|必填|音频地址|


##添加数据json格式
```
{
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
  "node": "node2",
  "programName":"G.E.M.邓紫棋 - 喜欢你.mp3"
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

