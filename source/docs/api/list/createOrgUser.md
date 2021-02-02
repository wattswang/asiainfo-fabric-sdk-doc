# 创建组织用户    

请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/organization/user/

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| OrganizationId |String |是 |组织Id| asiainfo-1tuigx42b|
| Username|String |是 |用户名| Username|
| Password|String |是 |密码| Password|
| Attrs|String |否 |ABAC属性| foo=foo1,bar=bar1|

返回数据
--------------------------------------------------------------------------

| 名称 | 类型 | 描述|示例值|
|-----|---  |---|----|
|RequestId| String |---|----|
|ErrorCode| Integer |---|----|
|Success| Boolean |---|----|
|Result| Object |---|----|

Result 正常返回示例
--------------------------------------------------------------------------
```
{
    "result": {
        "OrganizationId": "peers-yidio-1tuigx42b****",
        "CreateTime": "1999-05-10 09:00:00",
        "ExpireTime": "2000-05-10 09:00:00",
        "OrganizationName": "亚信科技",
        "Username": "username",
        "Password": "pwd"
    },
    "RequestId": "2537DB1B-F478-431E-A847-5DDAAE2BD251",
    "ErrorCode": 200,
    "Success": true
}
```