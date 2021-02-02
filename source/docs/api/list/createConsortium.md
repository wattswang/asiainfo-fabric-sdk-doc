# 创建联盟


请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/consortium/

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| OrdererType |String |是 |Orderer类型| raft|
| ConsortiumName|String |是 |联盟名| 崛起者联盟|
| ConsortiumDescription|Integer |是 |联盟描述| 为中华崛起|
| ChannelPolicy|String |是 |创建通道策略| Any|
| OrderersCount|Integer |是 |Orderer数量| 5|
| Organizations|String[] |是 |----|----- |
| OrganizationId|String |是 |组织ID| asiainfo-1tuigx42b1goc|


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
    "result":{
        "CodeName":"崛起者联盟",
        "ClusterState":"Pending",
        "ConsortiumId":"c-93k8d34jy79y79",
        "CreateTime":"1999-05-10 09:00:00",
        "OwnerBid":12312,
        "OrdererCount":1,
        "OrdererType":"kafka",
        "ConsortiumName":"崛起者联盟",
        "OrganizationCount":3,
        "ChannelCount":0,
        "ChannelPolicy":"ANY",
        "Description":"string",
        "Domain":"domain",
        "MemberCount":2,
        "ServiceState":"Pending"
    },
    "RequestId":"2537DB1B-F478-431E-A847-5DDAAE2BD251",
    "ErrorCode":200,
    "Success":true
}
```