
#标签管理列表
<font color="gray" size="3">@author：王云龙</font>

|METHOD|URI|
|--|--|
|GET|/hmf/operation/tag/simple/list|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|channelId|query|int|可选|频道ID|

## 响应
####响应成功
```
{
  "tagCount": 5,
  "channelCount": 4,
  "simpleHmfTags": [
    {
      "tagCount": "1",
      "channelName": "商业财经",
      "channelId": "65"
    },
    {
      "tagCount": "2",
      "channelName": "惊悚悬疑",
      "channelId": "59"
    },
    {
      "tagCount": "1",
      "channelName": "畅销小说",
      "channelId": "62"
    },
    {
      "tagCount": "1",
      "channelName": "都市",
      "channelId": "63"
    }
  ],
  "c": "s"
}
```