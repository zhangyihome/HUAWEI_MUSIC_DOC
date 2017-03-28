
#获取不同审核状态的节目数量
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/album/:albumId/reviewcount|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|


## 响应
```
{
  "albumReviewCountVO": {
    "totalCount": 13,
    "unReviewCount": 11,
    "reviewPassCount": 1,
    "reviewNotPassCount": 1
  },
  "c": "s"
}
```