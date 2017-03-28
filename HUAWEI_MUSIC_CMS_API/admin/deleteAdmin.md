# 删除用户
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|DELETE|/hmf/system/admin/admin/:admin|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|adminId|params|int|必须|adminId|--|

## 响应
####响应成功
```json
{
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

