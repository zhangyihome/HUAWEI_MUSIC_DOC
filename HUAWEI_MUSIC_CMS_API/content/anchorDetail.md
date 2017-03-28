
# 主播详情
<font color="gray" size="3">@author：许小宝</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/anchor/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|主 播ID|
## 响应
```
{
  "anchorVO": {
    "anchorUserId": 1,
    "userName": "testhu",
    "password": "123",
    "cpProperty": 2,
    "status": 1,
    "reviewStatus": 8,
    "reviewErrorId": 3,
    "reviewTime": "2017-03-20 11:19:50",
    "loginCount": 0,
    "companyName": "东方视角ww",
    "licenseUrl": "www.kting.cn",
    "realName": "果果",
    "nickName": "cc&dd",
    "phone": "1821095348825625635",
    "qqNumber": "1633537033",
    "wechat": "2",
    "provinces": "hubei",
    "city": "xiangyang",
    "address": "guyitown",
    "completeTime": "2017-03-17 18:20:17",
    "idcardUrl": "123",
    "idcardBackUrl": "456"
  },
  "c": "s"
}
```
