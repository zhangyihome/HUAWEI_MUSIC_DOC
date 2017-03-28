
# 专辑详情
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/album/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|专 辑ID|
## 响应
```
{
  "album": {
    "albumId": 1,	//专辑id
    "anchorUserId": 10,	//主播id
    "albumName": "胡泰然专辑1",	//专辑名称
    "albumType": 12,	//专辑类型
    "albumNickName": "测试修改昵称",	//专辑别名
    "channelId": 51,	//频道id
    "anchorName": "hutairan",	//主播名称
    "authorName": "asdf",	//作者名称
    "updateStatus": 21,	//更新状态
    "updateTime": "2017-03-22 13:20",	//最后更新时间
    "tags": "1,2,3",	//标签id串
    "tagList": [	//标签名列表
      "testTag",
      "tag3"
    ],
    "summary": "假数据",	//简介
    "agreementUrl": "123231231232",	//
    "status": 1,	//授权协议地址
    "reviewStatus": 8,	//审核状态
    "reviewErrorId": 0,	//审核不通过原因id
    "reviewTime": "2017-03-22 17:28",	//审核时间
    "audition": 10,	//试听数量
    "playProgramId": 2,	//默认播放id
    "defaultProgramName": "A-Lin - 给我一个理由忘记",	//默认播放节目名称
    "isRecommend": 15,	//是否推荐
    "onlineStatus": 20,	//上架状态
    "onlineTime": "2017-03-22 17:29",	//上架时间
    "offlineTime": "2017-03-22 17:29",	//下架时间
    "offlineErrorId": 35,	//下架原因
    "priceType": 24,	//定价类型
    "price": 1,	//价钱
    "sort": 1,	//排序序号
    "sortType": 26,	//专辑下节目列表排序类型
    "adminId": 1,	//后台用户id
    "createTime": "2017-03-15 18:37",	//创建时间
    "programNum": 13	//节目数量
  },
  "c": "s"
}
```
