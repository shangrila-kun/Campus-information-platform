http://domain/api/v1.0/crawler/list

```
后端展示爬虫程序
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190426 | 20190426 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | GET |
| **支持格式**     | application/x-www-form-urlencoded |
| **是否需要登录** | 否    |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述   |
| --------- | ---- | ---------- | ------ |
| sessionId | 是   | String     |        |

## 入参示例
```
{
	“sessionId" : "aaxxsegees"
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
    "result": [
        {
            "id": 1,
            "processName": "前方高能网站（资讯）",
            "version": "1",
            "status": "OFF",
            "processTag": "process_1",
            "taskCommand": null,
            "note": ""
        },
        {
            "id": 2,
            "processName": "前方高能网站（资源分享）",
            "version": "1",
            "status": "ON",
            "processTag": "process_2",
            "taskCommand": null,
            "note": null
        }
    ],
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
> id: 序号,
> processName: 程序名称
> version：当前版本号
> status: 程序状态 ON代表启动中 ，OFF代表关闭中
> processTag: 程序标志
> taskCommand: 任务命令,
> note: 备注

**展示爬虫程序时只需展示前四项内容即可**

