http://localhost:8089/data-sharing/comment/insertComment

## 功能描述
```
提交留言信息
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190310 | 20190310 |

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
| newsId    | 是   | Integer    | 新闻id   |
| content   | 是   | String     | 留言内容 |
| uEmail    | 是   | String     | 用户邮箱 |
| note      | 否   | String     | 备注     |

## 入参示例
```js
{
	"sessionId":"C1E23BCF1EB333F8DDF4E7E1126B1B58",
	"newsId":51,
	"content":"文章很棒",
	"uEmail":"11"
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
    "message": "操作成功"
}
```

```java
{
    "code": "500",
    "message": "无访问权限,请登录!"
}
```



---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
~~~

