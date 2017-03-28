
# 主播审核
<font color="gray" size="3">@author：许小宝</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/content/anchor/:anchorUserId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|anchorUserId|params|int|必须|主 播ID|
|status|body|int|必须|账号状态(1：开通:2：冻结)|
|statusErrorId|body|int|非必须|账号冻结原因|
|reviewStatus|body|int|必须|审核状态:8：通过:9：未通过)|
|reviewErrorId|body|int|非必须|审核不通过原因|
## 响应
```
{
  "c": "s"
}
```
