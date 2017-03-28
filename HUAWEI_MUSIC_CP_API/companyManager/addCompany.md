
# 添加机构信息
<font color="gray" size="3">@author：吴梦佳</font>

|METHOD|URI|
|--|--|
|POST|/amp/company/add|

## 参数

|名称|位置|类型|约束|描述|
|--|--|--|--|
|cpProperty|body|Integer|必须|用户性质（个人13、公司14）|
|companyName|body|String|必须|公司名称|
|licenseUrl|body|String|必须|营业执照照片地址|
|nickName|body|String|必须|推广名称|
|phone|body|String|必须|联系电话|
|qqNumber|body|String|必须|qq|
|wechat|body|String|非必须|微信|
|provinces|body|String|必须|省份|
|city|body|String|必须|城市|
|address|body|String|非必须|详细地址|



## 响应
####响应成功
```json
{
  "c": "s"
}
```
####系统错误
```json
{
  "c": "f",
  "i": "系统错误"
}
```
#### 参数错误
```json
{
  "c": "f",
  "i": "参数错误"
}
```
