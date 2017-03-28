# 获取热门电台列表
@author：段振超   
## 功能说明   
获取热门电台的内容列表
## 接口定义  
```
public <T extends BaseVO> void getHitAlbumList(int pageNo, int pageSize, int cachePolicy,
    final IResultCallBack<T> listener, final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getHitAlbumList(pageNo,pageSize,cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|pageNo|是|int|当前请求内容的页码|
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
      "albumId": 1381,
      "albumType": 11,
      "albumName": "呜呜呜呜呜呜无",
      "anchorName": "李四",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170103/23yx71s1.jpg",
      "playNum": 90121
    },
    {
      "albumId": 2367,
      "albumType": 12,
      "albumName": "基督教",
      "anchorName": "人人",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170106/249a36rm.jpg",
      "playNum": 109614
    },
    {
      "albumId": 132,
      "albumType": 12,
      "albumName": "吴晓波频道",
      "anchorName": "吴晓波",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161226/23d1gdih.jpg",
      "playNum": 77131
    }
  ],
  "c": "s"
}
```
