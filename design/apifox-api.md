# meditation

exported at 2024-03-27 22:56:07

## <p>

<p>
前端控制器
</p>


---
### 查询当前登录用户的所有achieve

> BASIC

**Path:** /achieve/list

**Method:** GET

**Desc:**

 查询当前登录用户的所有achieve

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
| data | array | 数据 |
| &ensp;&ensp;&#124;─ | object |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─id | integer |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─name | string |  |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": 0,
      "name": ""
    }
  ]
}
```




---
### 新增achieve

> BASIC

**Path:** /achieve

**Method:** POST

**Desc:**

 新增achieve

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| id | integer |  |
| name | string |  |

**Request Demo:**

```json
{
  "id": 0,
  "name": ""
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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 根据id查询achieve

> BASIC

**Path:** /achieve/{id}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ------------ | ------------ | ------------ |
| id |  |  |



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
| &ensp;&ensp;&#124;─id | integer |  |
| &ensp;&ensp;&#124;─name | string |  |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "id": 0,
    "name": ""
  }
}
```




---
### 根据id修改achieve

> BASIC

**Path:** /achieve

**Method:** PUT

**Desc:**

 根据id修改achieve

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| id | integer |  |
| name | string |  |

**Request Demo:**

```json
{
  "id": 0,
  "name": ""
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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 根据id删除achieve

> BASIC

**Path:** /achieve

**Method:** DELETE

**Desc:**

 根据id删除achieve

> REQUEST

**Query:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| id |  | NO |  |



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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```





## <p>

<p>
 前端控制器
</p>


---
### 查询当前登录用户的所有flower

> BASIC

**Path:** /flower/list

**Method:** GET

**Desc:**

 查询当前登录用户的所有flower

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
| data | array | 数据 |
| &ensp;&ensp;&#124;─ | object |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─id | integer |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─name | string |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─price | integer |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─totalRaindrop | integer |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─everydayRaindrop | integer |  |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": 0,
      "name": "",
      "price": 0,
      "totalRaindrop": 0,
      "everydayRaindrop": 0
    }
  ]
}
```




---
### 新增flower

> BASIC

**Path:** /flower

**Method:** POST

**Desc:**

 新增flower

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| id | integer |  |
| name | string |  |
| price | integer |  |
| totalRaindrop | integer |  |
| everydayRaindrop | integer |  |

**Request Demo:**

```json
{
  "id": 0,
  "name": "",
  "price": 0,
  "totalRaindrop": 0,
  "everydayRaindrop": 0
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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 根据id查询flower

> BASIC

**Path:** /flower/{id}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ------------ | ------------ | ------------ |
| id |  |  |



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
| &ensp;&ensp;&#124;─id | integer |  |
| &ensp;&ensp;&#124;─name | string |  |
| &ensp;&ensp;&#124;─price | integer |  |
| &ensp;&ensp;&#124;─totalRaindrop | integer |  |
| &ensp;&ensp;&#124;─everydayRaindrop | integer |  |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "id": 0,
    "name": "",
    "price": 0,
    "totalRaindrop": 0,
    "everydayRaindrop": 0
  }
}
```




---
### 根据id修改flower

> BASIC

**Path:** /flower

**Method:** PUT

**Desc:**

 根据id修改flower

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| id | integer |  |
| name | string |  |
| price | integer |  |
| totalRaindrop | integer |  |
| everydayRaindrop | integer |  |

**Request Demo:**

```json
{
  "id": 0,
  "name": "",
  "price": 0,
  "totalRaindrop": 0,
  "everydayRaindrop": 0
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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 根据id删除flower

> BASIC

**Path:** /flower

**Method:** DELETE

**Desc:**

 根据id删除flower

> REQUEST

**Query:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| id |  | NO |  |



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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 查询当前登录用户的所有learnrecords

> BASIC

**Path:** /learnrecords/list

**Method:** GET

**Desc:**

 查询当前登录用户的所有learnrecords

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
| data | array | 数据 |
| &ensp;&ensp;&#124;─ | object |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─userId | integer |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─studyTime | string |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─duration | integer |  |
| &ensp;&ensp;&ensp;&ensp;&#124;─studyStatus | integer |  |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "userId": 0,
      "studyTime": "",
      "duration": 0,
      "studyStatus": 0
    }
  ]
}
```




---
### 新增learnrecords

> BASIC

**Path:** /learnrecords

**Method:** POST

**Desc:**

 新增learnrecords

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| userId | integer |  |
| studyTime | string |  |
| duration | integer |  |
| studyStatus | integer |  |

**Request Demo:**

```json
{
  "userId": 0,
  "studyTime": "",
  "duration": 0,
  "studyStatus": 0
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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 根据userId查询learnrecords

> BASIC

**Path:** /learnrecords/{userId}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ------------ | ------------ | ------------ |
| userId |  |  |



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
| &ensp;&ensp;&#124;─userId | integer |  |
| &ensp;&ensp;&#124;─studyTime | string |  |
| &ensp;&ensp;&#124;─duration | integer |  |
| &ensp;&ensp;&#124;─studyStatus | integer |  |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
    "userId": 0,
    "studyTime": "",
    "duration": 0,
    "studyStatus": 0
  }
}
```




---
### 根据userId修改learnrecords

> BASIC

**Path:** /learnrecords

**Method:** PUT

**Desc:**

 根据userId修改learnrecords

> REQUEST

**Headers:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| Content-Type | application/json | YES |  |

**Request Body:**

| name | type | desc |
| ------------ | ------------ | ------------ |
| userId | integer |  |
| studyTime | string |  |
| duration | integer |  |
| studyStatus | integer |  |

**Request Demo:**

```json
{
  "userId": 0,
  "studyTime": "",
  "duration": 0,
  "studyStatus": 0
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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---
### 根据userId删除learnrecords

> BASIC

**Path:** /learnrecords

**Method:** DELETE

**Desc:**

 根据userId删除learnrecords

> REQUEST

**Query:**

| name | value | required | desc |
| ------------ | ------------ | ------------ | ------------ |
| userId |  | NO |  |



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

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```

-----------

### 查询所有的user

> BASIC

**Path:** /user/list

**Method:** GET

**Desc:**

 查询所有的user

> REQUEST



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                            | type    | desc                           |
| ----------------------------------------------- | ------- | ------------------------------ |
| code                                            | integer | 编码：1成功，0和其它数字为失败 |
| msg                                             | string  | 错误信息                       |
| data                                            | array   | 数据                           |
| &ensp;&ensp;&#124;─                             | object  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─id               | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─account             | string  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─password            | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─sunlight    | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─raindrop | integer |  
| &ensp;&ensp;&ensp;&ensp;&#124;─status | integer |        |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "id": 0,
      "account": "",
      "password": "",
      "sunlight": 0,
      "raindrop": 0,
      "status":0
    }
  ]
}
```




---

### 新增user

> BASIC

**Path:** /user

**Method:** POST

**Desc:**

 新增flower

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name     | type    | desc |
| -------- | ------- | ---- |
| id       | integer |      |
| account  | string  |      |
| password | integer |      |
| sunlight | integer |      |
| raindrop | integer |      |
| status   | integer |      |

**Request Demo:**

```json
 {
      "id": 0,
      "account": "",
      "password": "",
      "sunlight": 0,
      "raindrop": 0,
      "status":0
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id查询user

> BASIC

**Path:** /user/{id}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ---- | ----- | ---- |
| id   |       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                    | type    | desc                           |
| --------------------------------------- | ------- | ------------------------------ |
| code                                    | integer | 编码：1成功，0和其它数字为失败 |
| msg                                     | string  | 错误信息                       |
| data                                    | array   | 数据                           |
| &ensp;&ensp;&#124;─                     | object  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─id       | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─account  | string  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─password | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─sunlight | integer |                                |
| &ensp;&ensp;&#124;─status               | integer |                                |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
      "id": 0,
      "account": "",
      "password": "",
      "sunlight": 0,
      "raindrop": 0,
      "status":0
	}
}
```




---

### 根据id修改user

> BASIC

**Path:** /user

**Method:** PUT

**Desc:**

 根据id修改user

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name     | type    | desc |
| -------- | ------- | ---- |
| id       | integer |      |
| account  | string  |      |
| password | integer |      |
| sunlight | integer |      |
| raindrop | integer |      |
| status   | integer |      |

**Request Demo:**

```json
{
      "id": 0,
      "account": "",
      "password": "",
      "sunlight": 0,
      "raindrop": 0,
      "status":0
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id删除user

> BASIC

**Path:** /user

**Method:** DELETE

**Desc:**

 根据id删除user

> REQUEST

**Query:**

| name | value | required | desc |
| ---- | ----- | -------- | ---- |
| id   |       | NO       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 查询所有的userachieve

> BASIC

**Path:** /userachieve/list

**Method:** GET

**Desc:**

 查询所有的userachieve

> REQUEST



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                 | type    | desc                           |
| ------------------------------------ | ------- | ------------------------------ |
| code                                 | integer | 编码：1成功，0和其它数字为失败 |
| msg                                  | string  | 错误信息                       |
| data                                 | array   | 数据                           |
| &ensp;&ensp;&#124;─                  | object  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─user_id    | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─achieve_id  | string  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─get_time | integer |                                |


**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "user_id": 0,
      "achieve_id": 0,
      "get_time": ""
    }
  ]
}
```




---

### 新增userachieve

> BASIC

**Path:** /userachieve

**Method:** POST

**Desc:**

 新增userachieve

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name             | type    | desc |
| ---------------- | ------- | ---- |
| user_id          | integer |      |
| achieve_id       | string  |      |
| get_time         | integer |      |

**Request Demo:**

```json
{
      "user_id": 0,
      "achieve_id": 0,
      "get_time": ""
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id查询userachieve

> BASIC

**Path:** /userachieve/{id}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ---- | ----- | ---- |
| id   |       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                | type    | desc                           |
| ----------------------------------- | ------- | ------------------------------ |
| code                                | integer | 编码：1成功，0和其它数字为失败 |
| msg                                 | string  | 错误信息                       |
| data                                | object  | 数据                           |
| &ensp;&ensp;&ensp;&ensp;&#124;─user_id    | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─achieve_id  | string  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─get_time | integer |                                |


**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
      "user_id": 0,
      "achieve_id": 0,
      "get_time": ""
    }
}
```




---

### 根据id修改userachieve

> BASIC

**Path:** /userachieve

**Method:** PUT

**Desc:**

 根据id修改userachieve

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name       | type    | desc |
| ---------- | ------- | ---- |
| user_id    | integer |      |
| achieve_id | string  |      |
| get_time   | integer |      |

**Request Demo:**

```json
{
      "user_id": 0,
      "achieve_id": 0,
      "get_time": ""
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id删除userachieve

> BASIC

**Path:** /userachieve

**Method:** DELETE

**Desc:**

 根据id删除userachieve

> REQUEST

**Query:**

| name | value | required | desc |
| ---- | ----- | -------- | ---- |
| id   |       | NO       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 查询所有的userbuy

> BASIC

**Path:** /userbuy/list

**Method:** GET

**Desc:**

 查询所有的userbuy

> REQUEST



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                      | type    | desc                           |
| ----------------------------------------- | ------- | ------------------------------ |
| code                                      | integer | 编码：1成功，0和其它数字为失败 |
| msg                                       | string  | 错误信息                       |
| data                                      | array   | 数据                           |
| &ensp;&ensp;&#124;─                       | object  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─user_id    | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─flower_id | string  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─get_time   | integer |                                |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "user_id": 0,
      "flower_id": 0,
      "but_time": ""
    }
  ]
}
```




---

### 新增userbuy

> BASIC

**Path:** /userbuy

**Method:** POST

**Desc:**

 新增userbuy

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name             | type    | desc |
| ---------------- | ------- | ---- |
| user_id          | integer |      |
| flower_id        | string  |      |
| but_time         | integer |      |


**Request Demo:**

```json
{
      "user_id": 0,
      "flower_id": 0,
      "but_time": ""
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id查询userbuy

> BASIC

**Path:** /userbuy/{id}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ---- | ----- | ---- |
| id   |       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                | type    | desc                           |
| ----------------------------------- | ------- | ------------------------------ |
| code                                | integer | 编码：1成功，0和其它数字为失败 |
| msg                                 | string  | 错误信息                       |
| data                                | object  | 数据                           |
| &ensp;&ensp;&#124;─user_id               | integer |                                |
| &ensp;&ensp;&#124;─flower_id             | string  |                                |
| &ensp;&ensp;&#124;─but_time            | integer |                                |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
      "user_id": 0,
      "flower_id": 0,
      "but_time": ""
    }
}
```




---

### 根据id修改userbuy

> BASIC

**Path:** /userbuy

**Method:** PUT

**Desc:**

 根据id修改userbuy

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name             | type    | desc |
| ---------------- | ------- | ---- |
| user_id          | integer |      |
| flower_id        | string  |      |
| but_time         | integer |      |

**Request Demo:**

```json
{
      "user_id": 0,
      "flower_id": 0,
      "but_time": ""
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id删除userbuy

> BASIC

**Path:** /userbuy

**Method:** DELETE

**Desc:**

 根据id删除userbuy

> REQUEST

**Query:**

| name | value | required | desc |
| ---- | ----- | -------- | ---- |
| id   |       | NO       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 查询所有的userculture

> BASIC

**Path:** /userculture/list

**Method:** GET

**Desc:**

 查询所有的userculture

> REQUEST



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                      | type    | desc                           |
| ----------------------------------------- | ------- | ------------------------------ |
| code                                      | integer | 编码：1成功，0和其它数字为失败 |
| msg                                       | string  | 错误信息                       |
| data                                      | array   | 数据                           |
| &ensp;&ensp;&#124;─                       | object  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─user_id    | integer |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─flower_id | string  |                                |
| &ensp;&ensp;&ensp;&ensp;&#124;─culture_status   | integer |                                |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": [
    {
      "user_id": 0,
      "flower_id": 0,
      "culture_status": ""
    }
  ]
}
```




---

### 新增userculture

> BASIC

**Path:** /userculture

**Method:** POST

**Desc:**

 新增userculture

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name             | type    | desc |
| ---------------- | ------- | ---- |
| user_id               | integer |      |
| flower_id             | string  |      |
| culture_status            | integer |      |

**Request Demo:**

```json
{
      "user_id": 0,
      "flower_id": 0,
      "culture_status": ""
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id查询userculture

> BASIC

**Path:** /userculture/{id}

**Method:** GET

> REQUEST

**Path Params:**

| name | value | desc |
| ---- | ----- | ---- |
| id   |       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name                                | type    | desc                           |
| ----------------------------------- | ------- | ------------------------------ |
| code                                | integer | 编码：1成功，0和其它数字为失败 |
| msg                                 | string  | 错误信息                       |
| data                                | object  | 数据                           |
| &ensp;&ensp;&#124;─user_id               | integer |                                |
| &ensp;&ensp;&#124;─flower_id             | string  |                                |
| &ensp;&ensp;&#124;─culture_status            | integer |                                |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {
      "user_id": 0,
      "flower_id": 0,
      "culture_status": ""
    }
}
```




---

### 根据id修改userculture

> BASIC

**Path:** /userculture

**Method:** PUT

**Desc:**

 根据id修改userculture

> REQUEST

**Headers:**

| name         | value            | required | desc |
| ------------ | ---------------- | -------- | ---- |
| Content-Type | application/json | YES      |      |

**Request Body:**

| name             | type    | desc |
| ---------------- | ------- | ---- |
| user_id               | integer |      |
| flower_id             | string  |      |
| culture_status            | integer |      |

**Request Demo:**

```json
{
      "user_id": 0,
      "flower_id": 0,
      "culture_status": ""
}
```



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```




---

### 根据id删除userculture

> BASIC

**Path:** /userculture

**Method:** DELETE

**Desc:**

 根据id删除userculture

> REQUEST

**Query:**

| name | value | required | desc |
| ---- | ----- | -------- | ---- |
| id   |       | NO       |      |



> RESPONSE

**Headers:**

| name         | value                          | required | desc |
| ------------ | ------------------------------ | -------- | ---- |
| content-type | application/json;charset=UTF-8 | NO       |      |

**Body:**

| name | type    | desc                           |
| ---- | ------- | ------------------------------ |
| code | integer | 编码：1成功，0和其它数字为失败 |
| msg  | string  | 错误信息                       |
| data | object  | 数据                           |

**Response Demo:**

```json
{
  "code": 0,
  "msg": "",
  "data": {}
}
```


---

















