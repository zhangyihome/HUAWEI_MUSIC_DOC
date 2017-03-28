#获取订阅ID列表
@author：袁昊

##功能说明
获取订阅专辑的ID列表

##接口定义
```
public <T extends BaseVO> void getRssIds(int cachePolicy, final IResultCallBack<T> listener, final Class<T> clazz)
```

##接口调用说明
```
RequestApi.getRssIds(cachePolicy,listener,clazz)
```

##输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|cachePolicy|必须|int|缓存策略|
|listener|必须|IResultCallBack<T>|回调接口|
|clazz|必须|Class|回调接口泛型的实体类|

##返回类型说明
|返回类型|描述|
|--|--|
|RssIdListResult|回调结果实体类|

##回调结果说明
```
{
  "albumIdSet": [
    "1381",
    "2367",
    "132",
    "50",
    "58"
  ],
  "total": 0,
  "c": "s"
}
```