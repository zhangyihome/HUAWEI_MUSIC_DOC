
#修改专题
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/:subjectId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|subjectName|body|string|必须|专题名称|
|subjectCover|body|string|必须|专题封面|
|summary|body|string|必须|专题简介|
|abstracts|body|string|必须|专题摘要|

## 响应
####响应成功
```
{
  "c": "s"
}
```
####专题名称重复
```
{
  "c": "f",
  "i": "已经存在对应数据,不允许添加！"
}
```