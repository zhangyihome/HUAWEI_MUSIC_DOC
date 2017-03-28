#一些常量的定义

##说明
在RequestApi中定义了一些常量用于接口请求的参数

##静态常量定义
```
// 缓存策略
	/**
	 * 有cache先返cache,再请求net,再返net
	 */
	public static final int CACHE_CACHEANDNET = 0;
	/**
	 * 有cache先返cache,再请求net,不返net
	 */
	public static final int CACHE_CACHENONET = 1;
	/**
	 * 有cache先返cache,不再请求net,不返net，cache为空返回错误
	 */
	public static final int CACHE_ONLYCACHE = 2;
	/**
	 * 不返cache,请求net,返net
	 */
	public static final int CACHE_ONLYNET = 3;
	/**
	 * 不返cache,请求net,不返net只去缓存，下次备用
	 */
	public static final int CACHE_NO = 4;
```

```
// 请求列表数据每页的数据量
	/**
	 * 每页20条数据
	 */
	public static final int PAGESIZE_20 = 20;

	/**
	 * 每页30条数据
	 */
	public static final int PAGESIZE_30 = 30;
	
	/**
	 * 每页40条数据
	 */
	public static final int PAGESIZE_40 = 40;
```