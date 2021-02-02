# 获取联盟orderer节点信息

请求地址
--------------------------------------------------------------------------
GET /api/v1/namespaces/{namespace}/orderers/

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| ConsortiumId |String |是 |组织Id| asiainfo-1tuigx42b|

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
        "Result": [
            {
                "OrdererName": "order1",
                "Port": 7050,
                "Domain": "ordasdaerer1.orzxczcZXXweqwxsczxzXcxzxXzg1.alumunum.com",
                "CreateTime": "2020-07-01 09:00:00",
                "UpdateTime": "2020-07-02 09:00:00",
                "InstanceType": "ecs.n1.small"
            },
            {
                "OrdererName": "order2",
                "Port": 7050,
                "Domain": "orderer2.org1.alumunum.com",
                "CreateTime": "2020-07-01 09:00:00",
                "UpdateTime": "2020-07-02 09:00:00",
                "InstanceType": "ecs.n1.small"
            }
        ],
        "RequestId": "98B37CF5-AB0C-423E-8335-81A54899577E",
        "Success": true,
        "ErrorCode": 200
}
```