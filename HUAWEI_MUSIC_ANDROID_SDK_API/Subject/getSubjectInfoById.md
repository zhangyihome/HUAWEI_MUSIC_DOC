# 获取专题详情接口
@author：段振超
## 功能说明
获取指定id的专题的详情
## 接口定义
```
public static <T extends BaseVO> void getSubjectInfoById(long subjectId, int cachePolicy,
    final IResultCallBack<T> listener, final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getSubjectInfoById(subjectId,cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|subjectId|是|int|精选集id|
|cachePolicy|是|int|缓存策略|
|listener|是|IResultCallBack&lt;T&gt;|响应结果监听|
|clazz|是|Class&lt;T&gt;|接收数据的值对象|
##回调结果说明
#### 响应成功
```json

  {
  "subject": {
    "subjectId": 47,
    "subjectName": "ss",
    "summary": "ss",
    "introduction": "ss",
    "subjectCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/subject/cover/20170116/25327uav.jpg",
    "tags": "1484,1492,1493",
    "tagList": [
      {
        "tagId": 1484,
        "tagName": "圣斗士",
        "channelId": -1
      },
      {
        "tagId": 1492,
        "tagName": "wwwwwwwwwwwwwww",
        "channelId": -1
      },
      {
        "tagId": 1493,
        "tagName": "wwwwwwwwwwwwww",
        "channelId": -1
      }
    ],
    "albumListVO": [
      {
        "albumId": 2379,
        "albumType": 12,
        "albumName": "ssssss",
        "anchorName": "ssssss",
        "albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170116/252tp2ds.jpg"
      },
      {
        "albumId": 2380,
        "albumType": 11,
        "albumName": "sssss",
        "anchorName": "ss",
        "albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170116/252u155b.jpg"
      },
      {
        "albumId": 2380,
        "albumType": 11,
        "albumName": "sssss",
        "anchorName": "ss",
        "albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170116/252u155b.jpg"
      },
      {
        "albumId": 2379,
        "albumType": 12,
        "albumName": "ssssss",
        "anchorName": "ssssss",
        "albumCover": "http://192.168.2.207/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170116/252tp2ds.jpg"
      }
    ],
    "playNum": 125134
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
