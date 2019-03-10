http://localhost:8089/data-sharing/comment/getAllContents

## 功能描述
```
后台分页查询所有评论
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



| 参数名    | 必选 | 类型及范围 | 描述         |
| --------- | ---- | ---------- | ------------ |
| sessionId | 是   | String     |              |
| pageNum   | 是   | Integer    | 当前页数     |
| pageCount | 是   | Integer    | 每页显示几条 |

## 入参示例
```js
{
	"sessionId":"C1E23BCF1EB333F8DDF4E7E1126B1B58",
	"pageNum":1,
	"pageCount":10
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
    "message": "查询成功",
    "contents": [
        {
            "list": [
                {
                    "id": 7,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的非常很好",
                    "goodNums": "0",
                    "createTimeStamp": 1552221412
                },
                {
                    "id": 6,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的非常很好",
                    "goodNums": "0",
                    "createTimeStamp": 1552210902
                },
                {
                    "id": 5,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的非常很好",
                    "goodNums": "3",
                    "createTimeStamp": 1552210751
                },
                {
                    "id": 4,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的非常很好",
                    "goodNums": "0",
                    "createTimeStamp": 1552210588
                },
                {
                    "id": 3,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的非常很好",
                    "goodNums": "0",
                    "createTimeStamp": 1552210164
                },
                {
                    "id": 2,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的非常很好",
                    "goodNums": "0",
                    "createTimeStamp": 1552209978
                },
                {
                    "id": 1,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "这篇文章写的很好",
                    "goodNums": "1",
                    "createTimeStamp": 1552208781
                },
                {
                    "id": 8,
                    "uEmail": "11",
                    "newsId": 51,
                    "content": "文章很棒",
                    "goodNums": "0",
                    "createTimeStamp": 0
                }
            ],
            "size": 8
        }
    ]
}
```

```java
{
    "code": "500",
    "message": "无访问权限"
}
```



---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
~~~

