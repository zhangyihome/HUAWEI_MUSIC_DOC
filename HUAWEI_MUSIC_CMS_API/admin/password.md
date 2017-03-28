# 修改密码
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/system/admin/password|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|oldPassword|Body|String|必须|旧密码|--|
|oldPassword|Body|String|必须|新密码|--| 




## 请求参数
```json
{
	"oldPassword":"000000",
	"newPassword":"123456"
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


####密码错误
```json
{
  "c": "f",
  "i": "密码错误"
}
```
