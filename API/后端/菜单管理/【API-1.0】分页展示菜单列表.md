http://localhost:8089/data-sharing/menu/listAllMenu

```
后台分页展示所有菜单信息
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
                    "menuName": "大学生创业",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1541321953
                },
                {
                    "id": 6,
                    "menuName": "校园热点",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1541321953,
                    "note": "测试"
                },
                {
                    "id": 8,
                    "menuName": "竞赛信息",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1541321953,
                    "note": "测试"
                },
                {
                    "id": 10,
                    "menuName": "公益信息",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1544094951,
                    "note": "测试"
                },
                {
                    "id": 11,
                    "menuName": "资料分享",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1544095041,
                    "note": "测试"
                },
                {
                    "id": 12,
                    "menuName": "游戏娱乐",
                    "menuPriority": 8,
                    "isView": 1,
                    "createTimeStamp": 1544095441,
                    "note": "测试"
                },
                {
                    "id": 13,
                    "menuName": "游戏娱乐",
                    "menuPriority": 8,
                    "isView": 0,
                    "createTimeStamp": 1544100727,
                    "note": "测试"
                },
                {
                    "id": 14,
                    "menuName": "游戏娱乐",
                    "menuPriority": 8,
                    "isView": 0,
                    "createTimeStamp": 1544100796,
                    "note": "测试"
                },
                {
                    "id": 15,
                    "menuName": "游戏娱乐",
                    "menuPriority": 8,
                    "isView": 0,
                    "createTimeStamp": 1544102755,
                    "note": "测试"
                },
                {
                    "id": 16,
                    "menuName": "游戏娱乐",
                    "menuPriority": 8,
                    "isView": 0,
                    "createTimeStamp": 1544102766,
                    "note": "测试"
                }
            ],
            "size": 29
        }
    ]
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
无