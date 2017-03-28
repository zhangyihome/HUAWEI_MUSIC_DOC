
# 删除
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|DELETE|/hmf/operation/recommend/fourGrid/del/:position/:albumId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|params|int|必须|专辑id|
|position|params|int|必须|四宫格位置1,2,3,4|

## 响应
```
{
  "c": "s"
}
```
