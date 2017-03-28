
# 修改排序类型
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/channel/album/update/sortType|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|body|int|必须|专辑id|
|sortType|body|int|必须|正序26  倒序27|

## 响应
```
{
  "c": "s"
}
```
