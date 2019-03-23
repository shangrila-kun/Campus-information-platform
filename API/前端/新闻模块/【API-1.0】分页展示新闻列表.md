http://localhost:8089/data-sharing/news/listNews

## 功能描述
```
展示前端菜单信息
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



| 参数名    | 必选 | 类型及范围 | 描述                                                |
| --------- | ---- | ---------- | --------------------------------------------------- |
| menuId    | 是   | Integer    | 当为1时，代表首页查询，其他menuId代表不同类型的新闻 |
| pageNum   | 是   | Integer    | 当前是第几页                                        |
| pageCount | 是   | Integer    | 每页显示多少个                                      |

## 入参示例
```
{"menuId":1,
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
```
{
    "code": "200",
    "contents": {
        "list": [
            {
                "id": 21,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544670880,
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
                "id": 20,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
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
                "id": 19,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544623350,
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
                "id": 18,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544102768,
                "contentSource": "天天快报",
                "menu": {
                    "id": 11,
                    "menuName": "资料分享",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1544095041,
                    "note": "测试"
                },
                "note": "note"
            },
            {
                "id": 17,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544102758,
                "contentSource": "天天快报",
                "menu": {
                    "id": 10,
                    "menuName": "公益信息",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1544094951,
                    "note": "测试"
                },
                "note": "note"
            },
            {
                "id": 16,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544100798,
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
                "id": 15,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544100729,
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
                "id": 14,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544095443,
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
                "id": 13,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544095043,
                "contentSource": "天天快报",
                "menu": {
                    "id": 8,
                    "menuName": "竞赛信息",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1541321953,
                    "note": "测试"
                },
                "note": "note"
            },
            {
                "id": 12,
                "newsTitle": "第二篇新闻报道",
                "newsContent": "hello content",
                "sourceBigCategory": "123",
                "sourceVisitNumber": 11,
                "systemVisitNumber": 0,
                "sourceCreateData": "2018-05-04",
                "systemTimeStamp": 1544094955,
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
        ],
        "size": 21
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
200 代表返回成功
500 代表待用失败
~~~

