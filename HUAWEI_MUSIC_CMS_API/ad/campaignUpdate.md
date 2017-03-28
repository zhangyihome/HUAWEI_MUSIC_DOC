
# 修改广告活动
<font color="gray" size="3">@author:张春玲</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/ad/info/campaigns/:id|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|id|params|int|必须|广告活动ID|
|campaignName|Body|String|必须|广告活动名称|
|position|Body|short|必须|广告投放位置（151：电台首页_广告位1，152：电台首页_广告位2）|
|scheduleStart|Body|String|必须|排期开始时间|
|scheduleEnd|Body|String|必须|排期结束时间|
|scheduleList|Body|`List<String>`|必须|排期明细|
|weight|Body|short|必须|权重（范围1~9）|
|urlType|Body|short|必须|链接地址类型（161：外链，162：专辑，163：专题）|
|url|Body|String|必须|链接地:（urlType=162时为专辑ID，urlType=163时为节目ID）|
|scheme|Body|String|必须|广告文案，限制到20个字符 |
|creativeUrl|Body|String|必须|广告素材图片地址 |
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