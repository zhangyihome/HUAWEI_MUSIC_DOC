
# 修改审核状态
<font color="gray" size="3">@author:张春玲</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/content/album/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|专辑ID|
|reviewStatus|Body|int|必须|审核状态（8：审核通过，9：审核不通过）|
|reviewErrorId|Body|int|非必须|审核不通过原因|
## 响应
####响应成功
```
{
    "c":"s"
}
```
####响应失败
```
{
    "c":"f",
    "i":"参数错误！"
}
```