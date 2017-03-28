# 获取频道内容列表接口
@author：段振超   
## 功能说明   
获取指定频道的专辑列表
## 接口定义  
```
public static <T extends BaseVO> void getChannel(int channelId, int pageNo, int pageSize, int cachePolicy,
			final IResultCallBack<T> listener, final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getChannel(channelId,pageNo,pageSize,cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|channelId|是|int|频道id|
|pageNo|是|int|当前请求内容的页数|
|pageSize|是|int|每页数据条数|
|cachePolicy|是|int|缓存策略|
|listener|是|IResultCallBack&lt;T&gt;|响应结果监听|
|clazz|是|Class&lt;T&gt;|接收数据的值对象|


##回调结果说明
#### 响应成功  
```json
{
  "albumList": [
    {
      "albumId": 1,
      "albumType": 11,
      "albumName": "测试",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/subject/cover/20161124/yshk92q.jpg",
      "playNum": 0
    },
    {
      "albumId": 4,
      "albumType": 11,
      "albumName": "宋小宝第一步作品",
      "albumCover": "http://www.baidu.com/",
      "playNum": 0
    },
    {
      "albumId": 11,
      "albumType": 12,
      "albumName": "但是风格谁的风格",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170103/2412crj3.jpg",
      "playNum": 0
    }
  ],
  "c": "s"
}
```
