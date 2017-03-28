#标签列表
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/tag/tagList/:channelId|

## 参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|channelId|params|int|必须|频道ID|
## 响应
####响应成功
```
{
  "pagelist": [
    {
      "tagId": 2,
      "tagName": "testTag",
      "channelId": 59
    },
    {
      "tagId": 3,
      "tagName": "tag3",
      "channelId": 59
    }
  ],
  "total": 2,
  "c": "s"
}}
```
####响应失败
```
{
  "c": "f",
  "i": "没有找到符合条件的数据"
}
```