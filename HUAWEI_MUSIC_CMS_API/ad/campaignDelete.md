
# 删除广告活动
<font color="gray" size="3">@author：张春玲</font>

|METHOD|URI|
|--|--|
|DELETE|/hmf/ad/info/campaigns/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|广告活动ID|
## 响应
####响应成功
```
{
  "c": "s"
}
```
####响应失败
```
{
    "c":"f",
    "i":"参数错误！"
}
```