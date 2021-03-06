http://localhost:8089/data-sharing/resource/deleteResource

## 功能描述
```
后台删除资源，此删去并非真的从数据库删去，而是将状态isView设置为-1
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190412 | 20190412 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | GET   |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述     |
| --------- | ---- | ---------- | -------- |
| sessionId | 是   | String     |          |
| id        | 是   | Integer    | 当前页数 |

## 入参示例
```js
{
	"sessionId":"2E50DC7E6E3C8B43DCF5CB0E835F991A",
	"id":43
}
```

---

## 返回值说明
| 参数名   | 类型及范围 | 描述     |
| -------- | ---------- | -------- |
| code     | String     | 返回代码 |
| message  | String     | 返回信息 |
| contents | String     | 返回内容 |

## 返回值示例
```json
{
    "code": "200",
    "contents": "删除成功"
}
```

```java
{
    "code": "500",
    "contents": "删除失败"
}
```



---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
~~~

