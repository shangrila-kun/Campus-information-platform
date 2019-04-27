http://localhost:8888/api/v1.0/crawler/update/{id}/

```
后端控制爬虫程序是否开启
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190426 | 20190426 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | PUT |
| **支持格式**     | application/x-www-form-urlencoded |
| **是否需要登录** | 是 |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述   |
| --------- | ---- | ---------- | ------ |
| sessionId | 是   | String     |        |
| id      | 是   | Integer | 爬虫程序id |
| status | 是 | String | 程序状态（ON代表开启，OFF代表关闭） |

## 入参示例
```
{
	“sessionId" : "aaxxsegees"，
	"id":1,
	"status":ON
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

#### 成功

```
{
    "result": "OFF",
    "msg": "success",
    "code": 1
}
```

#### 失败（-1 代表没有调用权限 ，0代表操作失败）

```
{
    "result": null,
    "msg": "no permission",
    "code": -1
}
```
---

## 补充说明
> 1. 如果技术可行，建议采用前端控制开关按钮。可参考：<https://blog.csdn.net/hani_wen/article/details/80862608>
> 2. 该接口的请求方式为PUT方式，其中参数id 属于接口中的部门路径信息。发起ajax请求时，可以参考：<https://bbs.csdn.net/topics/391959284>

