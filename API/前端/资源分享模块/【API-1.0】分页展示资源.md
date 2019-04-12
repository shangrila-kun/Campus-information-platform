http://localhost:8089/data-sharing/resource/listResource

## 功能描述
```
展示前端资源分享模块
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



| 参数名    | 必选 | 类型及范围 | 描述           |
| --------- | ---- | ---------- | -------------- |
| pageNum   | 是   | Integer    | 当前是第几页   |
| pageCount | 是   | Integer    | 每页显示多少个 |

## 入参示例
```
{
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
```
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
                    "visitNums": 170,
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
                    "visitNums": 187,
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
                    "visitNums": 375,
                    "createTime": 1553319485,
                    "title": "title",
                    "url": "url",
                    "isView": 1
                },
                {
                    "id": 18,
                    "content": "我是用户3 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享2",
                    "type": "电子书资源",
                    "user": {
                        "uId": 3,
                        "uName": "xiu",
                        "uPassword": "123",
                        "uEmail": "xiu@qq.com",
                        "uStatus": "1",
                        "uRank": 0,
                        "uMotto": "我是一个好孩子"
                    },
                    "goodNums": 0,
                    "visitNums": 381,
                    "createTime": 1553315204,
                    "isView": 1
                },
                {
                    "id": 19,
                    "content": "我是用户1 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享3",
                    "type": "其他",
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
                    "visitNums": 381,
                    "createTime": 1553315204,
                    "isView": 1
                },
                {
                    "id": 20,
                    "content": "我是用户2 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享4",
                    "type": "源码资源",
                    "user": {
                        "uId": 2,
                        "uName": "22",
                        "uPassword": "22",
                        "uEmail": "22",
                        "uStatus": "1",
                        "uRank": 0,
                        "uMotto": ""
                    },
                    "goodNums": 0,
                    "visitNums": 381,
                    "createTime": 1553315204,
                    "isView": 1
                },
                {
                    "id": 21,
                    "content": "我是用户3 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享5",
                    "type": "视频资源",
                    "user": {
                        "uId": 3,
                        "uName": "xiu",
                        "uPassword": "123",
                        "uEmail": "xiu@qq.com",
                        "uStatus": "1",
                        "uRank": 0,
                        "uMotto": "我是一个好孩子"
                    },
                    "goodNums": 0,
                    "visitNums": 381,
                    "createTime": 1553315204,
                    "isView": 1
                },
                {
                    "id": 22,
                    "content": "我是用户1 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享6",
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
                    "visitNums": 320,
                    "createTime": 1553315204,
                    "isView": 1
                },
                {
                    "id": 23,
                    "content": "我是用户2 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享7",
                    "type": "其他",
                    "user": {
                        "uId": 2,
                        "uName": "22",
                        "uPassword": "22",
                        "uEmail": "22",
                        "uStatus": "1",
                        "uRank": 0,
                        "uMotto": ""
                    },
                    "goodNums": 0,
                    "visitNums": 319,
                    "createTime": 1553315204,
                    "isView": 1
                },
                {
                    "id": 24,
                    "content": "我是用户3 因为分享是一项传统美德，是一项生活技能，与人分享快乐，能使别人更快乐，自己也快乐。这是我的分享8",
                    "type": "源码资源",
                    "user": {
                        "uId": 3,
                        "uName": "xiu",
                        "uPassword": "123",
                        "uEmail": "xiu@qq.com",
                        "uStatus": "1",
                        "uRank": 0,
                        "uMotto": "我是一个好孩子"
                    },
                    "goodNums": 0,
                    "visitNums": 221,
                    "createTime": 1553315204,
                    "isView": 1
                }
            ],
            "size": 18
        }
    ]
}
```

```
{
    "code": "500",
    "message": "参数格式不合法"
}
```
---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
goodNums 代表点赞数，本模块暂时不实现点赞功能
visitNums 代表浏览器，建议使用
createTime 代表发布时间，时间戳类型
显示xx发布的，可以从user对象中获取用户信息。

资源分享模块：建议前台至少展示以下内容：
资源的标题：title
资源的摘要：content
资源的创建时间：createTime
资源的访问次数：visitNums
其中，点击标题跳转至：url
~~~

