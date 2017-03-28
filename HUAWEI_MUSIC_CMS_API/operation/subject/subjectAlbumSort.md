
#专题下专辑排序
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/:subjectId/album/:albumId/sort|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|albumId|param|int|必须|专辑ID|
|sort|body|int|必须|序号|

##数据json格式
```
{"sort":3}
```

## 响应
####响应成功
```
{
  "c": "s"
}
```