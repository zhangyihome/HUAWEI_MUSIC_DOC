
# 添加广告活动
<font color="gray" size="3">@author:张春玲</font>

|METHOD|URI|
|--|--|
|POST|/hmf/ad/info/campaigns/material|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|uploadFile|body|MultipartFile|必须|图片|

## 响应
####响应成功
```
{
  "fileVO": {
    "filePath": "/data/webapps/nginx/res/upload/cdn/default/cmsAd/material/20170327/2apiu88q.jpg",
    "webUrl": "http://192.168.2.206/res/upload/cdn/default/cmsAd/material/20170327/2apiu88q.jpg",
    "fileNewName": "2apiu88q.jpg",
    "fileOrigName": "桌面壁纸.jpg",
    "fileSize": 71039,
    "flag": 0
  },
  "audioInfoVO": null,
  "callBackVO": null,
  "fileVOList": null,
  "audioVOList": null,
  "c": "s",
  "i": null
}
```
