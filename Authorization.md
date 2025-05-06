# 获取Token

Uri：/api/authorize

Method：POST

## 参数

| 名称   | 类型   | 是否必须 | 描述   |
| :----- | :----- | :------- | :----- |
| key    | String | 是       | Key    |
| secret | String | 是       | Secret |

## 响应参数

| 名称         | 类型   | 描述                 |
| :----------- | :----- | :------------------- |
| access_token | String | Token                |
| token_type   | String | bearer               |
| expires_in   | Number | 过期时间（默认30天） |
