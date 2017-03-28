# 主页内容请求接口
@author：段振超   
## 功能说明   
获取首页内容
## 接口定义  
```
public static <T extends BaseVO> void getHomePageList(int cachePolicy, final IResultCallBack<T> listener,
			final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getHomePageList(cachePolicy,listener,clazz)
```
## 输入参数说明
|参数名称|是否必须|类型|描述|
|--|--|--|--|
|cachePolicy|是|int|缓存策略|
|listener|是|IResultCallBack&lt;T&gt;|响应结果回调|
|clazz|是|Class&lt;T&gt;|接收数据的值对象|
##回调结果说明
#### 响应成功  
```json
{
  "homePage": {
    "hitAlbumList": [
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
    "todayAlbumList": [
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
    "hitProgramList": [
      {
        "programId": 4,
        "albumId": 3,
        "programName": "宋小宝专辑",
        "programCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram2/cover/program/20161125/yv1avqk.jpg",
        "audioUrl": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/audio/convert/20161125/yvb48i5.mp3",
        "anchorName": "宋晓峰ggg66",
        "playNum": 78274,
        "duration": 0,
        "fileSize": 0
      },
      {
        "programId": 3,
        "albumId": 3,
        "programName": "郭德纲专辑",
        "programCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram2/cover/program/20161125/yv1avqk.jpg",
        "audioUrl": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/audio/convert/20161125/yv8burw.mp3",
        "anchorName": "宋晓峰ggg66",
        "playNum": 65267,
        "duration": 0,
        "fileSize": 0
      },
      {
        "programId": 39,
        "albumId": 3,
        "programName": "大幅度",
        "programCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/cmsProgram123456/cover/program/20161207/21u4wqfd.jpg",
        "audioUrl": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/audio/convert/20161207/21u4wy45.mp3",
        "anchorName": "宋晓峰ggg66",
        "playNum": 64786,
        "duration": 0,
        "fileSize": 0
      }
    ],
    "subjectList": [
      {
        "subjectId": 17,
        "subjectName": "测试郁金香",
        "introduction": "测试",
        "subjectCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/subject/cover/20161206/21rjtcpu.jpg",
        "playNum": 41116
      },
      {
        "subjectId": 31,
        "subjectName": "天下无贼2016最后一期",
        "introduction": "天下无贼天下无贼天下无贼天下无贼",
        "subjectCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/subject/cover/20161212/228qa6sq.jpg",
        "playNum": 824544
      },
      {
        "subjectId": 23,
        "subjectName": "爱情",
        "introduction": "发地方地方大幅度",
        "subjectCover": "http://192.168.2.195/res/upload/cdn/kting_huawei_fm/subject/cover/20161208/21w5rwjr.png",
        "playNum": 0
      }
    ]
  },
  "c": "s"
}
```
