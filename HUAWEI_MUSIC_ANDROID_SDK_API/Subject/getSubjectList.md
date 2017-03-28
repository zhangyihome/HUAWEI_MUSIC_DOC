# 获取专题列表接口
@author：段振超   
## 功能说明   
获取专题的内容列表
## 接口定义  
```
public <T extends BaseVO> void getSubjectList(int pageNo, int pageSize, int cachePolicy,
			final IResultCallBack<T> listener, final Class<T> clazz)
```
## 接口调用说明
```
RequestApi.getSubjectList(pageNo,pageSize,cachePolicy,listener,clazz)
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
  ],
  "c": "s"
}
```
