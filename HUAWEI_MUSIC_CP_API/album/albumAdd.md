# 添加专辑
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|POST|/amp/album/albums|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumCover|body|string|必须|专辑封面|
|albumName|body|string|必须|专辑名称|
|anchorName|body|string|必须|主播名称|
|authorName|body|string|非必须|作者名称|
|updateStatus|body|int|必须|更新状态(21,22)|
|channelId|body|int|必须|频道ID|
|tags|body|string|非必须|标签ID(1,2,3)|
|copyrightUrlList|body|string[]|必须|版权证明照片地址|
|agreementUrl|body|string|必须|授权协议照片地址|
|summary|body|string|必须|简介|
|programList|body|List<ProgramVO>|必须|节目（参见表1）|

## 表1

|名称|位置|类型|约束|描述|
|--|--|--|--|
|audio|Body|AudioInfoVO|必填|音频信息（参见表audio）|
|file|Body|FileVO|必填|文件信息（参见表file）|
|node|body|string|必须|上传节点|

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
	"albumName":"胡泰然专辑8",
	"anchorName":"hutairan",
	"albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser_10/album/cover/20170322/2aa5dpgc.png",
	"updateStatus":21,
	"channelId":59,
	"agreementUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser_10/album/cover/20170322/2aa5dpgc.png",
	"copyrightUrlList":[ "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser_10/album/cover/20170322/2aa5dpgc.png", "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser_10/album/cover/20170322/2aa5dpgc.png"],
	"summary":"假数据",
	"programList":[
	{
		"file": {
    		"filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5qmsb.mp3",
    		"webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5qmsb.mp3",
    		"fileNewName": "2aa5qmsb.mp3",
    		"fileOrigName": "F.I.R. - 你的微笑.mp3",
    		"fileSize": 10825869
		},
		"audio": {
    		"duration": 261500,
    		"bitRate": 320,
    		"samplingRate": 44100,
    		"format": "mp3",
    		"channels": 2
		},
		"node": "node1"
	},
	{
		"file": {
    		"filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5sey4.mp3",
    		"webUrl": "http://192.168.2.206/res/upload/cdn/kting_huawei_fm/ampUser10/audio/original/20170322/2aa5sey4.mp3",
    		"fileNewName": "2aa5sey4.mp3",
    		"fileOrigName": "F.I.R. - 月牙湾.mp3",
    		"fileSize": 12879852
		},
		"audio": {
    		"duration": 308500,
    		"bitRate": 320,
    		"samplingRate": 44100,
    		"format": "mp3",
    		"channels": 2
		},
		"node": "node2"
	}
	
	]
}
```
## 响应
```
{
  "c": "s"
}
```