
# 预览个人信息
<font color="gray" size="3">@author：吴梦佳</font>

|METHOD|URI|
|--|--|
|GET|/amp/person/detail|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|





## 响应
####响应成功
```json
{
  "personVO": {
    "anchorUserId": 3,
    "cpProperty": 13,
    "realName": "果",
    "nickName": "123",
    "phone": "18210953488",
    "qqNumber": "1633537033",
    "wechat": "2",
    "provinces": "beijing",
    "city": "xiangyang",
    "address": "guyitown",
    "idcardUrl": "123",
    "idcardBackUrl": "456",
    "reviewStatus":"7",
    "reviewErrorId":"0"
  },
  "c": "s"
}
```
####系统错误
```json
{
  "c": "f",
  "i": "系统错误"
}
```
#### 参数错误
```json
{
  "c": "f",
  "i": "参数错误"
}
```
