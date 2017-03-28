# 创建角色
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|POST|/hmf/system/role/role|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|roleName|Body|String|必须|角色名|--|
|roleExplain|Body|String|必须|角色说明|--|
|authList|Body|Object|必须|权限列表|--|



##请求参数
```json
{
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
