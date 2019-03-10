http://localhost:8089/data-sharing/advertisement/getAdvertisementsBypage

```
后台分页展示所有广告
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190310 | 20190310 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | POST  |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述           |
| --------- | ---- | ---------- | -------------- |
| sessionId | 是   | String     |                |
| pageNum   | 是   | Integer    | 当前是第几页   |
| pageCount | 是   | Integer    | 每页显示多少个 |

## 入参示例
```
{
	"sessionId":"52BF062CBC6D69EBFFDAD909E9BFAC31",
	"pageNum":1,
	"pageCount":10
}
```

---

## 返回值说明
| 参数名      | 类型及范围  | 描述   |
| -------- | ------ | ---- |
| code     | String | 返回代码 |
| message  | String | 返回信息 |
| contents | String | 返回内容 |

## 返回值示例
```
{
    "code": "200",
    "message": "查询成功",
    "contents": [
        {
            "list": [
                {
                    "id": 2,
                    "title": "我是广告Sun Mar 10 11:45:28 CST 2019",
                    "link": "www.baidu.com",
                    "isView": 1,
                    "priority": 6,
                    "createTimeStamp": 1552189528,
                    "note": "note"
                },
                {
                    "id": 1,
                    "title": "好好学习",
                    "link": "www.baidu.com",
                    "isView": 1,
                    "priority": 5,
                    "createTimeStamp": 0,
                    "note": "hello"
                },
                {
                    "id": 3,
                    "title": "我是广告Sun Mar 10 11:46:07 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189567,
                    "note": "note"
                },
                {
                    "id": 4,
                    "title": "我是广告Sun Mar 10 11:46:40 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189600,
                    "note": "note"
                },
                {
                    "id": 5,
                    "title": "我是广告Sun Mar 10 11:46:40 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189600,
                    "note": "note"
                },
                {
                    "id": 6,
                    "title": "我是广告Sun Mar 10 11:46:40 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189600,
                    "note": "note"
                },
                {
                    "id": 7,
                    "title": "我是广告Sun Mar 10 11:46:40 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189600,
                    "note": "note"
                },
                {
                    "id": 8,
                    "title": "我是广告Sun Mar 10 11:46:40 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189600,
                    "note": "note"
                },
                {
                    "id": 9,
                    "title": "我是广告Sun Mar 10 11:46:41 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189601,
                    "note": "note"
                },
                {
                    "id": 10,
                    "title": "我是广告Sun Mar 10 11:46:41 CST 2019",
                    "link": "www.ifeng.com",
                    "isView": 1,
                    "priority": 2,
                    "createTimeStamp": 1552189601,
                    "note": "note"
                }
            ],
            "size": 22
        }
    ]
}
```

```
{
    "code": "500",
    "message": "无访问权限",
    "contents": []
}
```
---

## 补充说明
无