
# 修改广告执行状态
<font color="gray" size="3">@author:张春玲</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/ad/info/campaigns/:id/status|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|广告活动ID|
|status|Body|short|必须|广告状态（153：暂停，154：执行）|
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