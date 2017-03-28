# 获取admin列表
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/hmf/system/role/role/:roleId|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|roleId|params|Integer|必须|角色id|--|




## 响应
####响应成功
```json
{
  "role": {
    "roleId": 2,
    "roleName": "test",
    "adminId": 1,
    "roleAuth": "{\"authList\":[{\"name\":\" 一级01\",\"url\":\"1234\",\"auth\":0,\"authList\":[{\"name\":\"01 二级 \",\"url\":\"1234\",\"auth\":1,\"authList\":[]}]},{\"name\":\" 一级02\",\"url\":\"1234\",\"auth\":1,\"authList\":[{\"name\":\"02 二级 01\",\"url\":\"1234\",\"auth\":1,\"authList\":[]},{\"name\":\"02 二级 02\",\"url\":\"1234\",\"auth\":1,\"authList\":[]}]}]}",
    "roleExplain": "测试修改"
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
