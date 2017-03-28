# 获取admin信息
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/hmf/system/admin/admin/:adminId|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|admin|params|Integer|必填|--|



## 响应
####响应成功
```json
{
  "admin": {
    "adminId": 3,
    "adminName": "韩立斌",
    "password": "2014a1ca34a51ead6465728764a10a95",
    "departmentId": "202",
    "roleId": 2,
    "createAdminId": 1
  },
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

####系统错误
```json
{
  "c": "f",
  "i": "系统错误"
}
```
