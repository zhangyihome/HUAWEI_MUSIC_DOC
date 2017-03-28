# 创建用户
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|POST|/hmf/system/admin/create|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|adminName|Body|String|必须|用户名|中文|
|departmentId|Body|String|必须|部门id|--| 
|roleId|Body|Int|必须|角色Id|列表未完善| 



## 请求参数
```json
{
	"adminName":"韩立斌",
	"departmentId":"201",
	"roleId":1
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


####账户名已存在
```json
{
  "c": "f",
  "i": "账户名已存在"
}
```
