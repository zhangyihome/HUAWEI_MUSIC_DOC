
#创建专题
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|POST|/hmf/operation/subject|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectName|body|string|必须|专题名称|
|subjectCover|body|string|必须|专题封面|
|summary|body|string|必须|专题简介|
|abstracts|body|string|必须|专题摘要|
|adminId|body|int|必须|创建人ID|

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