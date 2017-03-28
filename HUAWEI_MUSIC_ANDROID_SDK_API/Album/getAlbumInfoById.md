# 获取精选集详情接口
@author：段振超
## 功能说明
获取指定id的精选集的详情
## 接口定义
```
public <T extends BaseVO> void getAlbumInfoById(int albumId, int cachePolicy, final IResultCallBack<T> listener,
    final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getAlbumInfoById(albumId,cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|albumId|是|int|专辑id|
|cachePolicy|是|int|缓存策略|
|listener|是|IResultCallBack&lt;T&gt;|响应结果监听|
|clazz|是|Class&lt;T&gt;|接收数据的值对象|
##回调结果说明
#### 响应成功
```json
{
  "album": {
    "programNum": 0,
    "albumId": 50,
    "albumType": 12,
    "albumName": "赵本山小品修改",
    "summary": "赵本山第一部作品1",
    "playStatus": "0",
    "tags": "73",
    "tagList": [
      {
        "tagId": 73,
        "tagName": "杨过",
        "channelId": 64
      }
    ],
    "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161208/21wia213.jpg",
    "channelId": 51,
    "rssCount": 0
  },
  "c": "s"
}
```
```json
{
  "pageList": [
    {
      "programId": 55,
      "albumId": 32,
      "programName": "rap女伤感说唱 ",
      "programCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161207/21tth7bm.jpg",
      "audioUrl": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/audio/convert/20161207/21u72xnv.mp3",
      "playNum": 0,
      "duration": 96900,
      "fileSize": 775917
    },
    {
      "programId": 56,
      "albumId": 32,
      "programName": "rnb - 蓝调 - i still believe in love 甜美女声",
      "programCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161207/21tth7bm.jpg",
      "audioUrl": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/audio/convert/20161207/21u73nah.mp3",
      "playNum": 0,
      "duration": 96900,
      "fileSize": 775917
    },
    {
      "programId": 57,
      "albumId": 32,
      "programName": "艾薇儿666 iam with you",
      "programCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161207/21tth7bm.jpg",
      "audioUrl": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/audio/convert/20161207/21u72xrx.mp3",
      "playNum": 0,
      "duration": 223100,
      "fileSize": 1785527
    }
  ],
  "total": 0,
  "c": "s"
}
```
