# maozhuren
 猫主人社区

# 提交key 访问API 

1. 将开发者key加入到Http的Header里:
~~~ 
	GET  http://dengyun/v1/classic/latest
	 appkey: zCr1cd2jqewqeq 
~~~

2. 将开发者key作为请求参数 

~~~ 
   GET  http://dengyun/v1/classic/latest?appkey=zCr1cdeqweq
~~~
# 返回码

## HTTP 状态码

| 状态码 | 含义 | 说明 |
| --- | --- | --- |
| 200 | OK | 请求成功 |
| 201 | CREATED | 创建成功 |
| 202 | ACCEPTED | 更新成功 |
| 204 | NO CONTENT | 删除成功 |
| 301 | MOVED PERMANENTLY | 永久重定向 |
| 400 | BAD REQUEST | 请求包含不支持的参数 |
| 401 |  | 未授权 |
| 403 | FORBIDDEN | 被禁止访问 |
| 404 | NOT FOUND | 请求的资源不存在 |
| 413 | REQUIRED LENGTH TOO LARGE | 上传的File体积太大 |
| 500 | INTERNAL SERVER ERROR | 内部错误 |

## 错误码(error_code)

100x 通用类型:


| 错误码 | 含义 |
|---|---|
| 0 | OK, 成功 |
| 1000 | 输入参数错误 |
| 1001 | 输入的json格式不正确 |
| 1002 | 找不到资源 |
| 1003 | 未知错误 |
| 1004 | 禁止访问 |
| 1005 | 不正确的开发者key |
| 1006 | 服务器内部错误 |

200x 点赞类型

| 错误码 | 含义 |
| --- | --- |
| 2000 | 你已经点过赞了 |
| 2001 | 你还没点过赞 |

300x 期刊类型

| 错误码 | 含义 |
| --- | --- |
| 3000 | 该期内容不存在 |



