
# 修改专辑更新状态
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|PUT|/amp/album/:albumId/updateStatus|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|
|updateStatus|body|string|必须|更新状态(21,22)|


##添加数据json格式
```
{
	"updateStatus":22
}
```

## 响应
####响应成功
```
{
  "c": "s"
}
```
####响应失败
```
{
  "c": "f",
  "i": "参数错误！"
}
```