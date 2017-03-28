# 请求验证码
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/code/captcha/{phone}|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|phone|@PathVariable|String|必须|手机号|申请验证码的手机号|


## 响应
####响应成功
```json
{
  "secretKey": "eyJhbGciOiJIUzI1NiJ9.eyJqdGkiOi...",//验证码密钥，需要返回
  "captcha": "218203",//验证码，测试用后续删除
  "c": "s"
}
```

#### 手机号码错误
```json
{
  "c": "f",
  "i": "手机号码错误"
}
```
#### 发送失败
```json
{
  "c": "f",
  "i": "发送失败"
}
```

