# 获取验证码
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/code/kaptcha|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|



## 响应
####响应成功
```json
{
  "secretKey": "eyJhbGciOiJIUzI1NiJ9.eyJqdGkiOi...",//验证码密钥，需要返回
  "imageBase": "ata:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAAAeCAIAAABVO...",//验证码base数组
  "c": "s"
}
```


