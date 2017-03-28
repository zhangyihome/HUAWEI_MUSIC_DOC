# 获取节目列表接口
@author：段振超
## 功能说明
根据指定的专辑id获取其节目列表
## 接口定义
```
public static <T extends BaseVO> void getProgramListByAlbumId(int pageNo, int pageSize, int sort, int albumId,
			int cachePolicy, final IResultCallBack<T> listener, final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getProgramListByAlbumId(pageNo,pageSize,sort,albumId,cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|pageNo|是|int|当前请求内容的页码|
|pageSize|是|int|每页数据条数|
|sort|是|int|排序策略|
|albumId|是|int|专辑id|
|cachePolicy|是|int|缓存策略|
|listener|是|IResultCallBack&lt;T&gt;|响应结果监听|
|clazz|是|Class&lt;T&gt;|接收数据的值对象|
##回调结果说明
#### 响应成功
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
