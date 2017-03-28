#上传机构营业执照
<font color="gray" size="3">@author：吴梦佳</font>

|METHOD|URI|
|--|--|
|POST|/amp/company/upload/:uploadType|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|uploadType|params|String|必填|图片类型(companyCert)|
|uploadFile|form-data|MultipartFile|必填|图片文件|


## 响应
####响应成功
```
{
  "fileVO": {
    "filePath": "/data/webapps/nginx/res/upload/cdn/kting_huawei_fm/ampUser10/person/personCert/20170316/29sy3s9e.jpg",
    "webUrl": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/ampUser10/person/personCert/20170316/29sy3s9e.jpg",
    "fileNewName": "29sy3s9e.jpg",
    "fileOrigName": "2016.5大灰狼大刊 2.jpg",
    "fileSize": 496247
  },
  "c": "s"
}
```
####系统错误
```
{
  "c": "f",
  "i": "系统错误！"
}
```
####请求路径错误
```
{
  "c": "f",
  "i": "请求路径错误！"
}
```
####参数错误
```
{
  "c": "f",
  "i": "参数错误！"
}
```

