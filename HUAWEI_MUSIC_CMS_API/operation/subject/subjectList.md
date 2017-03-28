
#专题列表
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/subject/list/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|status|query|int|可选|上架状态(18:未上架，19:已上架，20:已下架)|
|sortType|query|int|可选|推荐状态(0:否，1:是)|
|condition|query|string|可选|查询条件（id:ID，subject:专题名称）|
|key|query|string|可选|查询关键字|

## 响应
####响应成功
```
{
  "total": 6,
  "hmfSubjects": [
    {
      "subjectId": 7,
      "subjectName": "测试专题名称7",
      "subjectCover": "http://192.168.1.2/test.jpg",
      "summary": "测试summary",
      "abstracts": "测试abstracts",
      "sortType": 15,
      "sort": 1,
      "updateTime": "2017-03-22 11:08:05",
      "adminId": 1,
      "createTime": "2017-03-22 10:44:55",
      "status": 18,
      "albumCount": 2
    },
    {
      "subjectId": 6,
      "subjectName": "测试专题名称6",
      "subjectCover": "http://192.168.1.2/test.jpg",
      "summary": "测试summary",
      "abstracts": "测试abstracts",
      "sortType": 15,
      "sort": 2,
      "updateTime": "2017-03-22 11:08:05",
      "adminId": 1,
      "createTime": "2017-03-22 10:34:47",
      "status": 18,
      "albumCount": 2
    },
    {
      "subjectId": 4,
      "subjectName": "测试专题名称4",
      "subjectCover": "http://192.168.1.2/test.jpg",
      "summary": "测试summary",
      "abstracts": "测试abstracts",
      "sortType": 15,
      "sort": 4,
      "updateTime": "2017-03-22 11:08:05",
      "adminId": 1,
      "createTime": "2017-03-20 16:46:02",
      "status": 19,
      "albumCount": 2
    },
    {
      "subjectId": 3,
      "subjectName": "测试专题名称3",
      "subjectCover": "http://192.168.1.2/test.jpg",
      "summary": "测试summary",
      "abstracts": "测试abstracts",
      "sortType": 15,
      "sort": 5,
      "updateTime": "2017-03-22 11:08:05",
      "adminId": 1,
      "createTime": "2017-03-20 16:24:57",
      "status": 19,
      "albumCount": 2
    },
    {
      "subjectId": 2,
      "subjectName": "测试专题名称2",
      "subjectCover": "http://192.168.1.2/test.jpg",
      "summary": "测试summary",
      "abstracts": "测试abstracts",
      "sortType": 15,
      "sort": 6,
      "updateTime": "2017-03-22 11:08:05",
      "adminId": 1,
      "createTime": "2017-03-20 16:11:00",
      "status": 18,
      "albumCount": 2
    },
    {
      "subjectId": 1,
      "subjectName": "测试专题名称1",
      "subjectCover": "http://192.168.1.2/test.jpg",
      "summary": "测试summary",
      "abstracts": "测试abstracts",
      "sortType": 16,
      "sort": 7,
      "updateTime": "2017-03-22 11:08:05",
      "adminId": 1,
      "createTime": "2017-03-20 10:38:14",
      "status": 19,
      "albumCount": 2
    }
  ],
  "c": "s"
}
```
####未查询到数据
```
{
  "c": "f",
  "i": "数据为空"
}
```