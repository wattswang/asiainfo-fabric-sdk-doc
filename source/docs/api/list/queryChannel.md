# 查询通道详情

请求地址
--------------------------------------------------------------------------
GET /api/v1/namespaces/{namespace}/channel/{channelId}

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| channelId |String |是 |通道ID| asiainfo-union-1tuigx42b|

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
    "Result":{
            "OrganizationName": "myorg",
            "InviteTime": "2018-07-23T01:53:53.000+0000",
            "ChannelId": "chan-cc1-2f0l9cd394****",
            "WithPeer": true,
            "OrganizationDescription": "",
            "OrganizationDomain": "zhuangADSADSDAACZXsdfadsdfaesfac1.absdasssample.cc",
            "State": "Accepted",
            "OrganizationId": "peers-zhuang1-2kna27h5m3c913",
            "AcceptTime": "2018-07-24T02:35:53.000+0000"
    },
    "RequestId": "3E85A941-658C-40E8-9704-60513A0281CF",
    "Success": true,
    "ErrorCode": 200
}
```