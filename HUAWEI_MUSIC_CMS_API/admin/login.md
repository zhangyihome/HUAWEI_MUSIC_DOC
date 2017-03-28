# 登陆
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|POST|/login/login|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|userName|Body|String|必须|用户名|--|
|password|Body|String|必须|密码|--| 
|captcha|Body|String|必须|验证码|--| 
|secretKey|Body|String|必须|秘钥|--| 


## 请求参数
```json
{
	"userName":"韩立斌",
	"password":"123456",
	"captcha":"8894",
	"secretKey":"eyJhbGciOiJIUzI1NiJ9.eyJqdGkiOi..."//验证码返回
}
```
## 响应
####响应成功
```json
{
  "admin": {
    "adminId": 3,
    "adminName": "韩立斌",
    "departmentId": "201",
    "roleId": 1,
    "createAdminId": 1
  },
  "token": "eyJhbGciOiJIUzI...".
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