# 获取电台排行榜的接口
@author：袁昊
## 功能说明
获取电台排行榜的四个榜单
## 接口定义
```
public static <T extends BaseVO> void getRankMap(int cachePolicy, final IResultCallBack<T> listener,
			final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getRankMap(cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|cachePolicy|是|int|缓存策略|
|listener|是|IResultCallBack&lt;T&gt;|响应结果监听|
|clazz|是|Class&lt;T&gt;|接收数据的值对象|

##返回类型说明
|返回类型|描述|
|--|--| 
|void||

##回调结果说明
#### 响应成功
```json
  {
  "rank": {
    "rankId": 0,
    "rankName": "分享最多",
    "rankType": 34,
    "albumList": [
      {
        "albumId": 5,
        "albumType": 12,
        "albumName": "但是风格谁的风格",
        "anchorName": "反跟",
        "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161201/21cimpjy.jpg"
      }
    ]
  },
  "c": "s"
}

```

#### 无返回值或报错
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
