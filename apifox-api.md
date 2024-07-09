# 员工管理

员工管理


---
## 登录

> BASIC

**Path:** /admin/employee/login

**Method:** POST

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| username | string | 用户名 |
| password | string | 密码 |

**Request Demo:**

```json
{
  "username": "",
  "password": ""
}
```



> RESPONSE

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| content-type | application/json;charset=UTF-8 | NO |  |

**Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg | string | 错误信息 |
| data | object | 数据 |
| &ensp;&ensp;&#124;─id | integer | 主键值 |
| &ensp;&ensp;&#124;─userName | string | 用户名 |
| &ensp;&ensp;&#124;─name | string | 姓名 |
| &ensp;&ensp;&#124;─token | string | jwt令牌 |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "id": 0,
    "userName": "",
    "name": "",
    "token": ""
  }
}
```




---
## 退出

> BASIC

**Path:** /admin/employee/logout

**Method:** POST

> REQUEST



> RESPONSE

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| content-type | application/json;charset=UTF-8 | NO |  |

**Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg | string | 错误信息 |
| data | string | 数据 |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": ""
}
```



