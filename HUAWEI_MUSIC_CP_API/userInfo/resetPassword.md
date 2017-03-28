# 忘记密码
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|PUT|/userInfo/password|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|userName|Body|String|必须|用户名|手机号|
|password|Body|String|必须|密码|--| 
|secretKey|Body|String|必须|密钥|验证码接口返回|
|captcha|Body|String|必须|验证码|--|

## 请求参数
```json
{
	"userName":"12345678904",
  "secretKey": "eyJhbGciOiJIUzI1NiJ9.eyJqdGkiOiJqd...",//密钥时效1分钟
  "captcha": "294083",
	"password":"123456"
}
```
## 备注

响应成功后，会在responesHeader中加入X-Auth-Token属性
token中携带用户基本信息

## 响应
####响应成功
```json
{
  "token": "eyJhbGciOiJIUzI1NiJ9.eyJqdGkiOiJqd3Qi...",
  "c": "s"
}
```

#### 系统错误
```json
{
  "c": "f",
  "i": "系统错误"
}
```

####参数错误
```json
{
  "c": "f",
  "i": "参数错误！"
}
```


####验证码不正确
```json
{
  "c": "f",
  "i": "验证码不正确"
}
```
####验证码过期
```json
{
  "c": "f",
  "i": "验证码过期"
}
```
