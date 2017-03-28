
#新建标签
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|POST|/hmf/operation/tag/:channelId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|channelId|params|int|必须|频道ID|
|tagName|body|string|必须|标签名称|
|adminId|body|int|必须|管理员ID|

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
  "i": "已经存在对应数据,不允许添加！"
}
```