
# 添加多个专辑
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|POST|/hmf/operation/recommend/fourGrid/add/multiple|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|albumId|body|int|必须|专辑id|
|position|body|int|必须|四宫格位置1,2,3,4|
|albumName|body|int|必须|专辑名称|

## 响应
```
{
  "addedNum": 0, //添加成功的数目
  "c": "s"
}
```
