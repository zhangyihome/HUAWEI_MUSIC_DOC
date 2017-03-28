
#修改专题推荐状态
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/:subjectId/sort/type|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|sortType|body|int|必须|专题推荐状态(15:正常，16:推荐，17:置顶)|

## 响应
####响应成功
```
{
  "c": "s"
}
```