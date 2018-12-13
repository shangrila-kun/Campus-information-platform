http://localhost:8089/data-sharing/news/getNewsByNewsId

## 功能描述
```
展示某篇新闻
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20181110 | 20181111 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | POST  |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名 | 必选 | 类型及范围 | 描述     |
| ------ | ---- | ---------- | -------- |
| id     | 是   | Integer    | 新闻的id |

## 入参示例
```
{"id":2}
```

---

## 返回值说明
| 参数名   | 类型及范围 | 描述     |
| -------- | ---------- | -------- |
| code     | String     | 返回代码 |
| message  | String     | 返回信息 |
| contents | String     | 返回内容 |

## 返回值示例
```
{
    "code": "201",
    "contents": {
        "id": 2,
        "newsTitle": "第二篇新闻报道",
        "newsContent": "hello content",
        "sourceBigCategory": "123",
        "sourceVisitNumber": 11,
        "systemVisitNumber": 0,
        "sourceCreateData": "2018-05-04",
        "systemTimeStamp": 1540804206,
        "contentSource": "天天快报",
        "menu": {
            "id": 2,
            "menuName": "大学生创业",
            "menuPriority": 8,
            "isView": 1,
            "createTimeStamp": 1541321953
        },
        "note": "note"
    }
}
```

```
{
    "code": "500",
    "message": "调用失败"
}
```
---

## 补充说明
~~~js
201 代表返回成功
500 代表待用失败
~~~

