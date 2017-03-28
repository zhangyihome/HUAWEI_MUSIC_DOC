#添加订阅
@author：袁昊

##功能说明
添加订阅

##接口定义
```
public static <T extends BaseVO> void addRss(long albumId, int cachePolicy, final IResultCallBack<T> listener,
			final Class<T> clazz) 
```

##接口调用说明
```
RequestApi.getRssList(albumId,cachePolicy,listener,clazz)
```

##输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|albumId|必须|long|专辑id|
|cachePolicy|必须|int|缓存策略|
|listener|必须|IResultCallBack<T>|回调接口|
|clazz|必须|Class|回调接口泛型的实体类|

##返回类型说明
|返回类型|描述|
|--|--| 
|void||

##回调结果说明
```
{
  "c": "s"
}
```