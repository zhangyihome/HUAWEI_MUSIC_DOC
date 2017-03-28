# 创建角色
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/system/role/role|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|roleId|Body|Integer|必须|角色Id|--|
|roleName|Body|String|必须|角色名|--|
|roleExplain|Body|String|必须|角色说明|--|
|authList|Body|Object|必须|权限列表|--|



##请求参数
```json
{
	"roleId":2
	"roleName":"test",
	"roleExplain":"测试",
	"authList":{
  "authList": [
    {
      "name": "系统",
      "url": "system",
      "auth":1,
      "authList": [
        {
          "name": "角色",
          "url": "role",
          "auth":1,
          "authList": []
        }
      ]
    },
    {
      "name": " 一级02",
      "authList": [
        {
          "name": "02 二级 01",
          "url": "1234",
          "auth":1,
          "authList": []
        },
        {
          "name": "02 二级 02",
          "url": "1234",
          "auth":1,
          "authList": []
        }
      ]
    }
  ]
}
}
```

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
