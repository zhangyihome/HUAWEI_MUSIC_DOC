#分页获取订阅列表
@author：袁昊

##功能说明
分页获取订阅列表

##接口定义
```
public static <T extends BaseVO> void getRssList(int pageNo, int pageSize, int cachePolicy,
			final IResultCallBack<T> listener, final Class<T> clazz)
```

##接口调用说明
```
RequestApi.getRssList(pageNo,pageSize,cachePolicy,listener,clazz)
```

##输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|pageNo|必须|int|第几页|
|pageSize|必须|int|每页多少数据|
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
  "pageList": [
    {
      "albumId": 58,
      "albumName": "流浪·欧罗巴的人",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161212/228xhqwf.jpg",
      "lastNum": 0,
      "updateNum": 0
    },
    {
      "albumId": 50,
      "albumName": "赵本山小品修改",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161208/21wia213.jpg",
      "lastNum": 0,
      "updateNum": 0
    },
    {
      "albumId": 132,
      "albumName": "吴晓波频道",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20161226/23d1gdih.jpg",
      "lastNum": 0,
      "updateNum": 0
    },
    {
      "albumId": 2367,
      "albumName": "基督教",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170106/249a36rm.jpg",
      "lastNum": 0,
      "updateNum": 0
    },
    {
      "albumId": 1381,
      "albumName": "呜呜呜呜呜呜无",
      "albumCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/album/20170103/23yx71s1.jpg",
      "lastNum": 0,
      "updateNum": 0
    }
  ],
  "total": 0,
  "c": "s"
}
```