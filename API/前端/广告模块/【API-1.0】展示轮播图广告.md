http://localhost:8089/data-sharing/advertisement/getViewAdvertisements

## 功能描述
```
前端轮播图展示
```
---
## 开发人员
| 人员     | 开始时间 | 结束时间 |
| -------- | :------: | :------: |
| **黄坤** | 20190310 | 20190310 |

## 调用方式

| Key              | Value |
| ---------------- | ----- |
| **HTTP请求方式** | GET   |
| **支持格式**     | JSON  |
| **是否需要登录** | 否    |

## 入参说明



| 参数名  | 必选 | 类型及范围 | 描述       |
| ------- | ---- | ---------- | ---------- |
| viewNum | 是   | Integer    | 展示的个数 |

## 入参示例
```js
{
	"viewNum":4
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
        [
            {
                "id": 2,
                "title": "我是广告Sun Mar 10 11:45:28 CST 2019",
                "imgsrc": "http://119.23.24.191:8080/1.jpg",
                "link": "http://119.23.24.191:8080/1.jpg",
                "isView": 1,
                "priority": 6,
                "createTimeStamp": 1552189528,
                "note": "note"
            },
            {
                "id": 1,
                "title": "好好学习",
                "imgsrc": "http://119.23.24.191:8080/2.jpg",
                "link": "www.baidu.com",
                "isView": 1,
                "priority": 5,
                "createTimeStamp": 0,
                "note": "hello"
            },
            {
                "id": 3,
                "title": "我是广告Sun Mar 10 11:46:07 CST 2019",
                "imgsrc": "http://119.23.24.191:8080/2.jpg",
                "link": "http://119.23.24.191:8080/2.jpg",
                "isView": 1,
                "priority": 2,
                "createTimeStamp": 1552189567,
                "note": "note"
            },
            {
                "id": 4,
                "title": "我是广告Sun Mar 10 11:46:40 CST 2019",
                "imgsrc": "http://119.23.24.191:8080/4.jpg",
                "link": "http://119.23.24.191:8080/3.jpg",
                "isView": 1,
                "priority": 2,
                "createTimeStamp": 1552189600,
                "note": "note"
            }
        ]
    ]
}
```



---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
~~~

