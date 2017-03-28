
# 下架
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/channel/album/update/offline|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|body|int|必须|专辑id|
|offlineTime|body|String|必须|下架时间|
|offlineErrorId|body|int|必须|下架原因:35版权已经到期  36内容质量差  37涉黄涉暴违规  38涉政违规  39版权有瑕疵  40其他|

## 响应
```
{
  "c": "s"
}
```
