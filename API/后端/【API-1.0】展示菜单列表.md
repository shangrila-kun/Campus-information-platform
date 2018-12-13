http://localhost:8089/data-sharing/menu/listAll

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



| 参数名 | 必选 | 类型及范围 | 描述 |
| ------ | ---- | ---------- | ---- |
|        |      |            |      |
|        |      |            |      |

## 入参示例
```
无
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
        [
            {
                "id": 1,
                "menuName": "首页",
                "menuPriority": 10,
                "isView": 1
            },
            {
                "id": 2,
                "menuName": "军事信息",
                "menuPriority": 8,
                "isView": 1
            },
            {
                "id": 3,
                "menuName": "经济新闻",
                "menuPriority": 6,
                "isView": 1
            },
            {
                "id": 6,
                "menuName": "学科竞赛",
                "menuPriority": 8,
                "isView": 0,
                "note": "测试"
            }
        ]
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