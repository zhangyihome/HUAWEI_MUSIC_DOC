
# 主播审核列表
<font color="gray" size="3">@author：许小宝</font>

|METHOD|URI|
|--|--|
|GET|/hmf/content/anchor/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|cpProperty|query|int|非必须|用户性质（13个人、14公司）|
|status|query|int|非必须|账号状态(1开通、2冻结)|
|reviewStatus|query|int|非必须|审核状态:（7：待审核，8：审核通过，9：审核未通过）|
|key|query|String|非必须|推广名称:(anchorUserId:用户ID,nickName:推广名称,userName:注册账号)|
|value|query|string|非必须|搜索值|
## 响应
```
{
  "list": [
    {
      "anchorUserId": 1,
      "userName": "testhu",
      "cpProperty": 2,
      "status": 1,
      "reviewStatus": 8,
      "reviewTime": "2017-03-20 11:19:50",
      "nickName": "cc&dd"
    },
    {
      "anchorUserId": 11,
      "userName": "12345678902",
      "status": 1
    },
    {
      "anchorUserId": 12,
      "userName": "12345678904",
      "status": 1
    },
    {
      "anchorUserId": 16,
      "userName": "12345678906",
      "status": 1,
      "reviewStatus": 7
    },
    {
      "anchorUserId": 10,
      "userName": "12345678901",
      "cpProperty": 13,
      "lastLoginTime": "2017-03-15 15:54:13",
      "status": 1,
      "reviewStatus": 8
    },
    {
      "anchorUserId": 18,
      "userName": "22222222222",
      "lastLoginTime": "2017-03-16 13:25:24",
      "status": 1,
      "reviewStatus": 7
    },
    {
      "anchorUserId": 19,
      "userName": "11111111189",
      "cpProperty": 13,
      "lastLoginTime": "2017-03-17 11:06:46",
      "status": 1,
      "reviewStatus": 7,
      "nickName": "12312"
    },
    {
      "anchorUserId": 17,
      "userName": "11111111111",
      "lastLoginTime": "2017-03-17 11:07:14",
      "status": 1,
      "reviewStatus": 7
    },
    {
      "anchorUserId": 15,
      "userName": "12345678905",
      "lastLoginTime": "2017-03-17 11:36:59",
      "status": 1,
      "reviewStatus": 7
    },
    {
      "anchorUserId": 21,
      "userName": "11111111789",
      "cpProperty": 14,
      "lastLoginTime": "2017-03-17 16:01:51",
      "status": 1,
      "reviewStatus": 7,
      "nickName": "123123"
    }
  ],
  "total": 20,
  "c": "s"
}
```
