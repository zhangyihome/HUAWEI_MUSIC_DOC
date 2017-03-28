# 修改用户
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/system/admin/admin|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|adminId|Body|int|必须|adminId|--|
|departmentId|Body|String|非必填|部门id|--| 
|roleId|Body|Int|非必填|角色Id|列表未完善| 



## 请求参数
```json
{
	"adminId":3,
	"departmentId":"202",
	"roleId":2
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


