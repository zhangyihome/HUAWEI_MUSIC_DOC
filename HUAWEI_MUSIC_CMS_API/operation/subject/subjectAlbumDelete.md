
#专题下删除专辑
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|DELETE|/hmf/operation/subject/:subjectId/album/:albumId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|albumId|param|int|必须|专辑ID|

## 响应
####响应成功
```
{
  "c": "s"
}
```