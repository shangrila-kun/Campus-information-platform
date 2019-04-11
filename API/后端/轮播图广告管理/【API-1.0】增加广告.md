http://localhost:8089/data-sharing/advertisement/insertAdvertisement

```
增加广告记录
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



| 参数名    | 必选 | 类型及范围 | 描述                              |
| --------- | ---- | ---------- | --------------------------------- |
| sessionId | 是   | String     |                                   |
| title     | 是   | String     | 广告名称                          |
| link      | 是   | String     | 广告链接                          |
|imgsrc|是|String|广告图片的地址，即
| isView    | 否   | Integer    | 1代表显示，0代表不显示，默认值为0 |
| priority  | 否   | Integer    | 默认值为5                         |
| note      | 否   | String     | 备注                              |

## 入参示例
```
{
	##待定
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
    "message": "操作成功"
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
