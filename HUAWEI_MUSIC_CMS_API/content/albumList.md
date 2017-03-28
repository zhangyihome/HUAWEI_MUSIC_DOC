
# 专辑审核列表
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/album/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|channelId|query|int|必须|频道ID|
|reviewStatus|query|int|必须|审核状态:（7：待审核，8：审核通过，9：审核未通过）|
|updateStatus|query|int|必须|更新状态（21：连载，22：完本）|
|key|query|String|非必须|关键词类型（albumId:专辑ID、albumName：专辑名、anchorName：主播名、albumNickName：推广名）|
|value|query|string|非必须|查询条件：搜索关键词|
## 响应
```
{
  "list": [
    {
      "albumId": 2, // 专辑ID
      "albumName": "胡泰然专辑2", // 专辑名称
      "albumNickName": "测", // 推广名称
      "anchorName": "hutairan", // 主播名称
      "channelId": 51, // 频道ID
      "updateStatus": 21, //更新状态
      "updateTime": "2017-03-17 09:52",// 更新时间
      "reviewStatus": 7, // 审核状态
      "createTime": "2017-03-16 09:54",// 审核时间
      "programNum": 3 //节目数
    }
  ],
  "total":1,
  "c": "s"
}
```
