http://localhost:8089/data-sharing/user/getUsers

```
后台分页展示普通用户信息
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
                    "uId": 3,
                    "uName": "xiu",
                    "uLegal": "1",
                    "uEmail": "xiu@qq.com",
                    "uStatus": "1",
                    "uRank": 0,
                    "uMotto": "我是一个好孩子"
                },
                {
                    "uId": 5,
                    "uName": "111",
                    "uLegal": "1",
                    "uEmail": "111@qq.com",
                    "uStatus": "1",
                    "uRank": 0,
                    "uMotto": "111"
                },
                {
                    "uId": 6,
                    "uName": "1111",
                    "uLegal": "1",
                    "uEmail": "111@qq.com",
                    "uStatus": "1",
                    "uRank": 0,
                    "uMotto": "1111"
                },
                {
                    "uId": 7,
                    "uName": "1111",
                    "uLegal": "1",
                    "uEmail": "111@qq.com",
                    "uStatus": "1",
                    "uRank": 0,
                    "uMotto": "1111"
                }
            ],
            "size": 6
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