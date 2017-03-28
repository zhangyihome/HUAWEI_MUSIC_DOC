#上传专辑协议
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|POST|/amp/album/agreement/:agreementType|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|agreementType|params|String|必填|上传图片位置(agreement、copyright)|
|uploadFile|form-data|MultipartFile|必填|图片文件|

## 参数说明
agreementType有且只有两个值
agreement 指的是授权协议
copyright 指的是版权证明

## 响应
####响应成功
```
{
  "fileVO": {
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg",
    "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/album/copyright/20170316/29sfmihr.jpg",
    "fileNewName": "29sfmihr.jpg",
    "fileOrigName": "u=1419900898,4156249374&fm=21&gp=0.jpg",
    "fileSize": 5867
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
