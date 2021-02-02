# 浏览账本信息

请求地址
--------------------------------------------------------------------------
GET /api/v1/namespaces/{namespace}/ledger/

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| OrganizationId |String |是 |组织Id| asiainfo-1tuigx42b|
| channelId|String |是 |通道ID| 通道ID|
| chaincodeId|String |是 |链码ID| 链码ID|
| Method|String |是 |密码| 方法|
| Body|String |否 |请求参数| 请求参数|

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
    "RequestId":"AB2560A0-EF98-462D-B9BA-D422206B94B3",
    "ErrorCode":200,
    "Success":true,
    "Result":"{}"
}
```