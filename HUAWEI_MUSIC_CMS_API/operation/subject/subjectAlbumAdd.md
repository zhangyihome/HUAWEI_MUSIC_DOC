
#专题下添加专辑
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|POST|/hmf/operation/subject/:subjectId/album|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|adminId|body|int|必须|创建人ID|
|albumsId|body|int[]|必须|专辑ID数组|

##数据json格式
```
{"adminId":1,"albumsId":[1,2,3]}
```

## 响应
####响应成功
```
{
  "c": "s",
  "i": "1,2,3添加失败"
}
```