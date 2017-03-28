# 获取admin列表
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/hmf/system/role/roles/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|pageNo|params|Integer|必须|页号|--|
|pageSize|params|Integer|必须|页大小|--|



## 响应
####响应成功
```json
{
  "pageList": [
    {
      "roleId": 4,
      "roleName": "test",
      "adminId": 0,
      "roleExplain": "测试"
    },
    {
      "roleId": 3,
      "roleName": "test",
      "adminId": 0,
      "roleExplain": "测试"
    },
    {
      "roleId": 1,
      "roleName": "test",
      "adminId": 0,
      "roleExplain": "测试"
    }
  ],
  "total": 3,
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
