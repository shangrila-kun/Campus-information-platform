http://localhost:8089/data-sharing/resource/listAllResource

## 功能描述
```
后台分页获取资源
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190412 | 20190412 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | GET   |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名    | 必选 | 类型及范围 | 描述           |
| --------- | ---- | ---------- | -------------- |
| sessionId | 是   | String     |                |
| pageNum   | 是   | Integer    | 当前页数       |
| pageCount | 是   | Integer    | 每页显示多少个 |

## 入参示例
```js
{
	"sessionId":"2E50DC7E6E3C8B43DCF5CB0E835F991A",
	"pageNum":1,
	"pageCount":10
}
```

---

## 返回值说明
| 参数名   | 类型及范围 | 描述     |
| -------- | ---------- | -------- |
| code     | String     | 返回代码 |
| message  | String     | 返回信息 |
| contents | String     | 返回内容 |

## 返回值示例
```json
{
    "code": "200",
    "message": "查询成功",
    "contents": [
        {
            "list": [
                {
                    "id": 42,
                    "content": "1",
                    "type": "校园竞赛类",
                    "user": {
                        "uId": 1,
                        "uName": "管理员",
                        "uPassword": "manager@1.com",
                        "uEmail": "manager@qq.com",
                        "uStatus": "0",
                        "uRank": 0,
                        "uMotto": "hello,i am uMotto。"
                    },
                    "goodNums": 0,
                    "visitNums": 169,
                    "createTime": 1554296499,
                    "title": "title",
                    "url": "url",
                    "isView": 1
                },
                {
                    "id": 39,
                    "content": "w",
                    "type": "电子书资源类",
                    "user": {
                        "uId": 1,
                        "uName": "管理员",
                        "uPassword": "manager@1.com",
                        "uEmail": "manager@qq.com",
                        "uStatus": "0",
                        "uRank": 0,
                        "uMotto": "hello,i am uMotto。"
                    },
                    "goodNums": 0,
                    "visitNums": 186,
                    "createTime": 1554294580,
                    "title": "title",
                    "url": "url",
                    "isView": 1
                },
                {
                    "id": 31,
                    "content": "这是我上传的点子书，大家可以点击下载，www.baidu.com",
                    "type": "电子书资源",
                    "user": {
                        "uId": 1,
                        "uName": "管理员",
                        "uPassword": "manager@1.com",
                        "uEmail": "manager@qq.com",
                        "uStatus": "0",
                        "uRank": 0,
                        "uMotto": "hello,i am uMotto。"
                    },
                    "goodNums": 0,
                    "visitNums": 374,
                    "createTime": 1553319485,
                    "title": "title",
                    "url": "url",
                    "isView": 1
                }
            ],
            "size": 18
        }
    ]
}
```

```java
{
    "code": "500",
    "contents": "操作失败"
}
```



---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败

资源分享模块：建议前台至少展示以下内容：
资源的标题：title
资源的摘要：content
资源的创建时间：createTime
资源的访问次数：visitNums
其中，点击标题跳转至：url

后台展示自定义
~~~

