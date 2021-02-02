# 获取组织详情

请求地址
--------------------------------------------------------------------------
GET /api/v1/namespaces/{namespace}/organization/{organizationId}

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| organizationId |String |是 |组织ID| asiainfo-1tuigx42b|

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
    "Result": {
        "OrganizationDescription": "organization created by ruiqi.zss",
        "Domain": "peer.aliyun.abasssample.cc",
        "ZoneId": "cn-shanghai-a",
        "OrganizationId": "org-ip92i26m792c9",
        "OrganizationName": "亚信科技",
        "ConsortiumCount": 1,
        "UserCount": 0,
        "State": "Created",
        "SpecName": "ecs.n1.medium",
        "OwnerUid": 1204281570282129,
        "CAUrl": "https://ca1.org1.alibabacloudbaas.com:31154",
        "CreateTime": "2018-06-22T06:14:21.000+0000",
        "CANAME": "caname",
        "CodeName": "aliyun",
        "OwnerName": "blockchain_baas_test",
        "PeerCount": 2,
        "OwnerBid": "26842"
    },
    "RequestId": "C445762C-8909-4BD8-A2BD-BB45BF2441D8",
    "Success": true,
    "ErrorCode": 200
}
```