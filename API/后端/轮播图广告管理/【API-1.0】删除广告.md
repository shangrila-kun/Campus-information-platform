http://localhost:8089/data-sharing/advertisement/deleteById

```
后台删除指定广告
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



| 参数名    | 必选 | 类型及范围 | 描述   |
| --------- | ---- | ---------- | ------ |
| sessionId | 是   | String     |        |
| id        | 是   | Integer    | 广告号 |

## 入参示例
```
{
	"sessionId":"52BF062CBC6D69EBFFDAD909E9BFAC31",
	"id":23
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
    "message": "删除成功"
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