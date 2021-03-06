http://localhost:8089/data-sharing/menu/deleteMenu

```
根据菜单id，删除菜单
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



| 参数名    | 必选 | 类型及范围 | 描述 |
| --------- | ---- | ---------- | ---- |
| id        | 是   | Integer    |      |
| sessionId | 是   | String     |      |

## 入参示例
```
{"id":9,
 "sessionId:"xxxxxxxxxdddddddddddd"
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
    "contents": "删除成功"
}
```

```
{
    "code": "500",
    "message": "删除失败"
}
```
---

## 补充说明
无