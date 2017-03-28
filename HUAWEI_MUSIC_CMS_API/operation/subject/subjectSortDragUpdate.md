
#专题拖拽排序
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/sort|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|list|body|List<HmfSubjectVO>|必须|后台接收一个List|

##数据json格式
```
[
  {"subjectId":1,"sort":7},
  {"subjectId":2,"sort":6}
]
```

## 响应
####响应成功
```
{
  "c": "s"
}
```