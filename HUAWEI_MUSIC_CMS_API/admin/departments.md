# 获取部门列表
<font color="gray" size="3">@author：韩立斌</font>

|METHOD|URI|
|--|--|
|GET|/hmf/system/admin/departments|

## 参数

|名称|位置|类型|约束|描述|备注|
|--|--|--|--|--|--|
|firstId|Paramter|Integer|非必填|一级部门Id|不填返回一级部门列表，填了返回对应的二级部门列表|



## 响应
####响应成功
```json
{
  "departments": [
    {
      "departmentId": 201,
      "departmentName": "研发中心"
    },
    {
      "departmentId": 202,
      "departmentName": "华为业务部"
    },
    {
      "departmentId": 203,
      "departmentName": "酷听业务部"
    },
    {
      "departmentId": 204,
      "departmentName": "渠道媒介部"
    },
    {
      "departmentId": 205,
      "departmentName": "综合辅助"
    }
  ],
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

####系统错误
```json
{
  "c": "f",
  "i": "系统错误"
}
```
