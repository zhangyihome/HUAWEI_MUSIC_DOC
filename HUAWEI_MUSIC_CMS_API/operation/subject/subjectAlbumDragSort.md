
#专题下专辑拖拽排序
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/subject/:subjectId/album/sort|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|subjectId|param|int|必须|专题ID|
|albumId|param|int|必须|专辑ID|
|list|body|List|必须|后台接收List|

##数据json格式
```
[{"subjectAlbumId":1,"sort":2},{"subjectAlbumId":2,"sort":1}]
```

## 响应
####响应成功
```
{
  "c": "s"
}
```