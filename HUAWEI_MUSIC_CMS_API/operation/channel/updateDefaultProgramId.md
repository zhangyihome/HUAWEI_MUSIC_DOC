
# 修改默认播放Id
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/channel/album/update/playProgramId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|body|int|必须|专辑id|
|playProgramId|body|int|必须|默认播放Id|

## 响应
```
{
  "c": "s"
}
```
