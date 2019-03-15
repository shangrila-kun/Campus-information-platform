http://localhost:8089/data-sharing/user/updateUserInfo

## 功能描述
```
普通用户更新
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

| 参数名 | 必选 | 类型及范围 | 描述                        |
| ------ | ---- | ---------- | --------------------------- |
| uId    | 是   | String     | 用户ID，用户id不可更新      |
| uEmail | 是   | String     | 用户邮箱，用户邮箱不可更新  |
| uSex   | 是   | Integer    | 0代表男，1代表女，3代表保密 |
| uName  | 是   | String     | 用户名称                    |
| uMotto | 是   | String     | 座右铭                      |
| uNote  | 否   | String     | 备注                        |

## 入参示例
```js
{
	"uId":1,
	"uName":"hk",
	"uSex":1,
	"uEmail":"266@.com",
	"uMotto":"hello,i am uMotto。",
	"sessionId": "ADAEEFBBE6108CB7A1E7FE43CFD009DB"
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
    "message": "更新成功"
}
```

```json
{
    "code": "500",
    "message": "更新失败"
}
```
~~~json
{
    "code": "501",
    "message": "无调用权限"
}
~~~



---

## 补充说明
~~~js
200 代表返回成功
500 代表待用失败
~~~

