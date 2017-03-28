
# 修改是否推荐
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/channel/album/update/recommend|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|body|int|必须|专辑id|
|isRecommend|body|int|必须|15正常  16推荐|

## 响应
```
{
  "c": "s"
}
```
