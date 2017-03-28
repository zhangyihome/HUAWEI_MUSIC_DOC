# 获取admin列表
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/hmf/system/admin/admins/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|pageNo|params|Integer|必须|页号|--|
|pageSize|params|Integer|必须|页大小|--|



## 响应
####响应成功
```json
{
  "pagelist": [
    {
      "adminId": 1,
      "adminName": "nihao",
      "password": "50cddbfcd2c316b449ddd7f1f18dd0ca",
      "departmentId": "201",
      "roleId": 1,
      "createAdminId": 1
    },
    {
      "adminId": 2,
      "adminName": "hahaha",
      "password": "719a8a68b57840132693db55dd0c3286",
      "departmentId": "201",
      "roleId": 1,
      "createAdminId": 1
    },
    {
      "adminId": 3,
      "adminName": "韩立斌",
      "password": "2014a1ca34a51ead6465728764a10a95",
      "departmentId": "202",
      "roleId": 2,
      "createAdminId": 1
    }
  ],
  "tatol": 3,
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
