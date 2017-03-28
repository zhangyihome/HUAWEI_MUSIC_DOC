
# 修改专辑
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|PUT|/amp/album/:albumId|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|
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

##添加数据json格式
```
{
	"albumName":"胡泰然专辑2",
	"anchorName":"hutairan",
	"albumCover":"http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/cover/album/20170316/29sbt9e1.png",
	"updateStatus":11,
	"tags":"1,2,3",
	"channelId":51,
	"agreementUrl":"http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/agreement/20170316/29sfj1xp.jpg",
	"copyrightUrlList":["http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg","http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/agreement/20170316/29sfj1xp.jpg"],
	"summary":"假数据"
}
```

## 响应
####响应成功
```
{
  "c": "s"
}
```
####响应失败
```
{
  "c": "f",
  "i": "专辑不能重名"
}
```