
# 上架
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/channel/album/update/online|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|body|int|必须|专辑id|
|onlineTime|body|String|必须|上架时间|
|priceType|body|int|必须|定价类型:23免费  24专辑  25多集|
|price|body|double|必须|定价|
|audition|body|int|必须|试听数量|

## 响应
```
{
  "c": "s"
}
```
