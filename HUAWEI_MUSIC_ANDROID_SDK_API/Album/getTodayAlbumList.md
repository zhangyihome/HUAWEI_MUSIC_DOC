# 获取今日必听列表接口
@author：段振超   
## 功能说明   
获取今日必听的内容列表
## 接口定义  
```
public <T extends BaseVO> void getTodayAlbumList(int pageNo, int pageSize, int cachePolicy,
			final IResultCallBack<T> listener, final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getTodayAlbumList(pageNo,pageSize,cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
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
      "albumId": 50,
      "albumType": 12,
      "albumName": "赵本山小品修改",
      "anchorName": "赵本山--范伟",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161208/21wia213.jpg",
      "playNum": 151015
    },
    {
      "albumId": 58,
      "albumType": 12,
      "albumName": "流浪·欧罗巴的人",
      "anchorName": "清文",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161212/228xhqwf.jpg",
      "playNum": 108524
    },
    {
      "albumId": 61,
      "albumType": 12,
      "albumName": "口才书",
      "anchorName": "口才书",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161212/228ykjgb.jpg",
      "playNum": 107003
    }
  ],
  "c": "s"
}
```
