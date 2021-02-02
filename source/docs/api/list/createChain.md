# 创建链码

请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/chaincode/

 请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| organizationId |String |是 |组织ID| org-asiainfo|
| channelId |String |是 |通道ID| channel-asiainfo-union-1w55v3u39x2xz|
| consortiumId |String |是 |联盟ID| consortium-asiainfo-union-akpcsjjac2jd|
| chaincodeUrl |String |是 |链码地址| /tmp/chains/test1.cc|
| endorsePolicy |String |是 |背书策略| 	OR ('asiainfoMSP.peer')|

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
    "result": [
        {
            "ChaincodeName": "sacc",
            "ChannelId": "chan-first-channel-1w55v3u39x2xz",
            "State": "Instantiatable",
            "ConsortiumId": "consortium-aaaaaa-akpcsjjac2jd",
            "Creator": "aaaaaa1",
            "CreateTime": 1544766801000,
            "Install": "true",
            "ChannelName": "channel-asiainfo-union",
            "ChaincodeVersion": "1.0",
            "EndorsePolicy": "OR (&#39;asiainfoMSP.peer&#39;)",
            "ChaincodeId": "code-sacc-1pr09q7jmo0np"
        }
    ],
    "requestId": "50B3ACF3-CE12-433C-A834-9E8C657A4934",
    "success": true,
    "errorCode": 200
 }
```
