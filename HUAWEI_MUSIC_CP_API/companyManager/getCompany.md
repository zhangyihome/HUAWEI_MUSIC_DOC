
# 预览机构信息
<font color="gray" size="3">@author：吴梦佳</font>

|METHOD|URI|
|--|--|
|GET|/amp/company/detail|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|




## 响应
####响应成功
```json
{
  "companyVO": {
    "anchorUserId": 3,
    "cpProperty": 14,
    "companyName": "东方视角",
    "licenseUrl": "www.kting.cn",
    "nickName": "568223121",
    "phone": "18210953488",
    "qqNumber": "1633537033",
    "provinces": "beijing",
    "city": "xiangyang",
    "address": "guyitown",
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
