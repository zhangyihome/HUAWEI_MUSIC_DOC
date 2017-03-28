
# 输入排序
<font color="gray" size="3">@author:张春玲</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/content/album/：albumId/inputSort|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|
|targetSort|Body|int|必填|目标元素序号|
|ownSort|Body|int|必填|被移元素序号|
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