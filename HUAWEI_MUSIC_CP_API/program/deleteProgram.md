# 删除节目
<font color="gray" size="3">@author：胡泰然</font>

|METHOD|URI|
|--|--|
|DELETE|/amp/program/:programId|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|programId|Params|int|必填|节目ID|



## 响应
####响应成功
```json
{
  "c": "s"
}
```

#### 参数错误
```json
{
  "c": "f",
  "i": "参数错误"
}
```

