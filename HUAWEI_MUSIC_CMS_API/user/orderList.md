
# 频道下专辑列表
<font color="gray" size="3">@author：王辉</font>

|METHOD|URI|
|--|--|
|GET|/hmf/user/order/findPage/:pageNo/:pageSize|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|pageNo|params|int|必须|当前页码|
|pageSize|params|int|必须|每页数据数目|
|key|query|string|非必须|key可以是:albumId albumName hwId cuid orderId|
|value|query|string|非必须|查询条件：搜索关键值|
## 响应
```
{
  "list": [
    {
      "id": 2,
      "orderId": "10001",	//订单id
      "cuid": "123",
      "hwId": "132",	//华为用户id
      "payType": 25,	//购买方式,等同于定价类型 23免费 24专辑 25多集
      "albumId": 32,	//专辑id
      "albumName": "就回家了",	//专辑名称
      "amount": 1,	//总价
      "status": 1,	//状态
      "cTime": "2017-03-27 12:37"	//下单时间
    }
  ],
  "total": 1,
  "c": "s"
}
```
