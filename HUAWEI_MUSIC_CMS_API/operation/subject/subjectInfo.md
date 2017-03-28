
#专题详情
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/subject/:subjectId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|params|int|必须|subjectId|

## 响应
####响应成功
```
{
  "subjectId": 3,
  "subjectName": "测试专题名称3",
  "subjectCover": "http://192.168.1.2/test.jpg",
  "summary": "测试summary",
  "abstracts": "测试abstracts",
  "sortType": 15,
  "sortTypeName": "正常",
  "sort": 5,
  "updateTime": "2017-03-22 11:08:05",
  "adminId": 1,
  "createTime": "2017-03-20 16:24:57",
  "status": 19,
  "statusInfo": "已上架",
  "c": "s"
}
```
####未查询到数据
```
{
  "c": "f",
  "i": "没有找到符合条件的数据"
}
```