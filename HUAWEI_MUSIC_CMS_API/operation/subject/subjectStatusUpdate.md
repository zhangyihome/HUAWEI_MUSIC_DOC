
#修改专题上下架状态
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/:subjectId/status|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|status|body|int|必须|专题上下架状态(19:上架，20:下架)|

## 响应
####响应成功
```
{
  "c": "s"
}
```