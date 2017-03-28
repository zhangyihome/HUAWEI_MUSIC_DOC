# 获取权限配置列表
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/hmf/system/role/authList|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|



## 响应
####响应成功
```json
{
  "authList": {
    "authList": [
      {
        "name": "系统设置",
        "url": "system",
        "auth": 0,
        "authList": [
          {
            "name": "用户管理",
            "url": "admin",
            "auth": 0
          },
          {
            "name": "角色管理",
            "url": "role",
            "auth": 0
          }
        ]
      }
    ]
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
