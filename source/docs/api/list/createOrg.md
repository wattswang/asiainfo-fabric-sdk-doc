# 创建组织

请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/organization/

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| OrganizationName |String |是 |组织名称| 亚信科技|
| Description|String |是 |描述| 为中华崛起|
| PeersCount|Integer |是 |节点数量| 5|

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
        "CodeName": "崛起者区块链联盟",
        "ClusterState": "Pending",
        "OrganizationId": "c-93k8d34jy79y79",
        "CreateTime": "1999-05-10 09:00:00",
        "OwnerBid": 12312,
        "OrganizationName": "亚信科技",
        "SpecName": "basic",
        "ConsortiumCount": 0,
        "PeerCount": 5,
        "Description": "string",
        "Domain": "domain",
        "UserCount": 2,
        "ServiceState": "Pending"
    },
    "RequestId": "2537DB1B-F478-431E-A847-5DDAAE2BD251",
    "ErrorCode": 200,
    "Success": true
}
```