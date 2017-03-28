
#获取不同审核状态的专辑数量
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|GET|/amp/album/reviewcount|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|


## 响应
```
{
  "albumReviewCountVO": {
    "totalCount": 6,              //总量
    "unReviewCount": 5,           //待审核数量
    "reviewPassCount": 1,         //审核通过数量
    "reviewNotPassCount": 0       //审核未通过数量
  },
  "c": "s"
}
```