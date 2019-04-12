http://localhost:8089/data-sharing/menu/editMenu

## 功能描述
```
后台编辑菜单，仅支持修改优先级和是否显示
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190412 | 20190412 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | POST  |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名       | 必选 | 类型及范围 | 描述             |
| ------------ | ---- | ---------- | ---------------- |
| sessionId    | 是   | String     |                  |
| id           | 是   | Integer    |                  |
| menuPriority | 是   | Integer    | 0-10             |
| isView       | 是   | Integer    | 0或者1,1代表显示 |

## 入参示例
```
{
	"sessionId":"2E50DC7E6E3C8B43DCF5CB0E835F991A",
	"id":66,
	"menuPriority":10,
	"isView":1
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
    "message": "修改成功",
}
```

```
{
    "code": "500",
    "message": "修改失败"
}
```
---

## 补充说明
无
