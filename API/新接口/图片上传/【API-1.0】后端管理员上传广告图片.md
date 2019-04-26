http://domain/api/v1.0/backend/file

```
后端上传广告图片
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190426 | 20190426 |

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
| 参数名 | 类型及范围 | 描述                    |
| ------ | ---------- | ----------------------- |
| code   | Integer    | 1代表成功，-1代表失败   |
| msg    | String     | 返回提示的信息          |
| result | String     | 返回上传成功后的文件url |

## 返回值示例

### 成功

```
{
    "result": "www.haoeasy.cn/images/8a9d9b5b-1057-43c8-b263-15e4bfa694a0.png",
    "msg": " upload success",
    "code": 1
}
```

### 失败（-1 代表没有调用权限 ，0代表操作失败）

```
{
    "result": null,
    "msg": "no permission",
    "code": -1
}
```
---

## 补充说明
无
