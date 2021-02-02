# 实例化链码

请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/chaincode/{chaincodeId}/instantiate

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| organizationId |String |是 |组织ID| org-asiainfo|
| channelId |String |是 |通道ID| channel-asiainfo-union-1w55v3u39x2xz|
| chaincodeId |String |是 |联盟ID| chan-channelx-1l1hmckuuisxo|
返回数据
--------------------------------------------------------------------------

| 名称 | 类型 | 描述|示例值|
|-----|---  |---|----|
|RequestId| String |---|----|
|ErrorCode| Integer |---|----|
|Success| Boolean |---|----|
|Result| Object |---|----|

正常返回示例
--------------------------------------------------------------------------
```
{
    "Result": {
        "install": false,
        "channelName": "mychannel",
        "input": "args:&quot;john&quot; args:&quot;10&quot; ",
        "ChaincodeName": "mycc3",
        "Path": "github.com/hyperledger/fabric-samples/chaincode/sacc",
        "state": "Running",
        "chaincodeId": "cc-198jejf8f8chi8",
        "type": 1,
        "ChaincodeVersion": "0.1",
        "ConsortiumId":"consortium-lianmenyumingyi-hc5d1bwlulg7",
        "CreateTime":"1533025590",
        "EndorsePolicy":"OR (perf9141MSP.member)",
        "Message":"OK"
    },
    "RequestId": "7D27692E-C501-4B1D-878C-0B869DD3D9E6",
    "Success": true,
    "ErrorCode": 200
}
```
