http://localhost:8089/data-sharing/upload/advertisement

```
上传广告图片
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
| **支持格式**     | form-data  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述   |
| --------- | ---- | ---------- | ------ |
| sessionId | 是   | String     |        |
| file        | 是   | file    | 图片 |

## 入参示例
```
{
	form-data形式，入参包括sessionId和file,可以百度查看vue上传图片代码,form-data 格式
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
    "message": "success",
    "contents": [
        "http://xxxxxxx:8080/img/20190408215736314237jpg"
    ]
}
```

```
{
    "code": "500",
    "message": "error",
   
}
```
---

## 补充说明
无
