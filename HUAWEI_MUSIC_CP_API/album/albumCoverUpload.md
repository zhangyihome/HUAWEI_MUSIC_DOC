#上传专辑封面
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|POST|/amp/album/cover|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|base64|Body|String|必填|上传的节目封面的bses64数组|

## 响应
####响应成功
```
{
  "fileVO": {
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/cmsProgram10/cover/album/20170316/29sbt9e1.png",
    "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram10/cover/album/20170316/29sbt9e1.png",
    "fileNewName": "29sbt9e1.png",
    "fileOrigName": "10album_cover.png",
    "fileSize": 94428
  },
  "c": "s"
}
```
####响应失败
```
{
  "c": "f",
  "i": "数据错误！"
}
```
