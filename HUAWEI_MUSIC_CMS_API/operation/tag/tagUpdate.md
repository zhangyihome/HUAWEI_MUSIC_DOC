
#修改标签
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/operation/tag/:channelId/:tagId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|channelId|params|int|必须|频道ID|
|tagId|params|int|必须|标签ID|
|tagName|body|string|必须|标签名称|

## 响应
####响应成功
```
{
  "c": "s"
}
```
####标签名重复
```
{
  "c": "f",
  "i": "已经存在对应数据！"
}
```