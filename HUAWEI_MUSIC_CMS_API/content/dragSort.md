
# 拖动排序
<font color="gray" size="3">@author:张春玲</font>

|METHOD|URI|
|--|--|
|PUT|/hmf/content/album/：albumId/dragSort|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑ID|
|list|Body|List<ProgramVO> list|必填|后台需要接受的一个list|

## ProgramVO参数
|名称|位置|类型|约束|描述|
|--|--|--|--|
|programId|Body|int|必填|节目ID|
|sort|Body|int|必填|排序字段|
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