# 登陆
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|POST|/userInfo/login|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|userName|Body|String|必须|用户名|手机号|
|password|Body|String|必须|密码|--| 


## 请求参数
```json
{
	"userName":"12345678901",
	"password":"654321"
}
```
## 响应
####响应成功
```json
{
  "user": {
    "anchorUserId": 15,
    "userName": "12345678905",
    "cpProperty": 0,
    "status": 1,
    "statusErrorId": 0,
    "reviewStatus": 0,
    "reviewErrorId": 0,
    "loginCount": 0
  },
  "token": "eyJhbGciOiJIUzI1N...",		//token
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


####账户名不存在
```json
{
  "c": "f",
  "i": "账户名不存在"
}
```

####密码错误
```json
{
  "c": "f",
  "i": "密码错误"
}
```