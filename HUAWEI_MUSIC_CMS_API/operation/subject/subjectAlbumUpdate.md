
#专题下修改专辑别名
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/:subjectId/album/:albumId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|albumId|param|int|必须|专辑ID|
|albumNickName|body|String|必须|专辑别名|

##数据json格式
```
{"albumNickName":"新专辑"}
```

## 响应
####响应成功
```
{
  "c": "s"
}
```