http://localhost:8080/data-sharing/news/getNewsByTitleFuzzyMatch

## 功能描述
```
根据新闻标题模糊查找
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20181212 | 20181214 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | POST  |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述     |
| --------- | ---- | ---------- | -------- |
| newsTitle | 是   | String     | 新闻标题 |

## 入参示例
```json
{
	"newsTitle":"第二篇"
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
```
{
    "code": "200",
    "contents": [
        {
            "id": 2,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1540804206,
            "contentSource": "天天快报",
            "menu": {
                "id": 1,
                "menuName": "首页",
                "menuPriority": 10,
                "isView": 1,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 15,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544100729,
            "contentSource": "天天快报",
            "menu": {
                "id": 3,
                "menuName": "大学生就业",
                "menuPriority": 6,
                "isView": 0,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 18,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544102768,
            "contentSource": "天天快报",
            "menu": {
                "id": 3,
                "menuName": "大学生就业",
                "menuPriority": 6,
                "isView": 0,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 20,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544624287,
            "contentSource": "天天快报",
            "menu": {
                "id": 2,
                "menuName": "大学生创业",
                "menuPriority": 8,
                "isView": 1,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 23,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544671989,
            "contentSource": "天天快报",
            "menu": {
                "id": 2,
                "menuName": "大学生创业",
                "menuPriority": 8,
                "isView": 1,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 24,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544673425,
            "contentSource": "天天快报",
            "menu": {
                "id": 2,
                "menuName": "大学生创业",
                "menuPriority": 8,
                "isView": 1,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 26,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544707382,
            "contentSource": "天天快报",
            "menu": {
                "id": 2,
                "menuName": "大学生创业",
                "menuPriority": 8,
                "isView": 1,
                "createTimeStamp": 1541321953
            },
            "note": "note"
        },
        {
            "id": 28,
            "newsTitle": "第二篇新闻报道",
            "newsContent": "hello content",
            "sourceBigCategory": "123",
            "sourceVisitNumber": 11,
            "systemVisitNumber": 3,
            "sourceCreateData": "2018-05-04",
            "systemTimeStamp": 1544708242,
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
        
    ]
}
```

```
{
    "code": "500",
    "message": "参数有误"
}
```
---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
~~~

