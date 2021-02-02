# 升级链码

请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/chaincode/{chaincodeId}/upgrade

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
        "ProviderId":"provider",
        "ProviderName":"name",
        "ChaincodeName": "mycc3",
        "Input": "args:&quot;john&quot; args:&quot;10&quot; ",
        "Install": false,
        "State": "Running",
        "Type": 1,
        "ChannelName": "mychannel",
        "ConsortiumId":"consortium-lianmenyumingyi-hc5d1bwl****",
        "ChaincodeVersion": "0.1",
        "ChaincodeId": "cc-null-c856k9i1m****",
        "Path": "github.com/hyperledger/fabric-samples/chaincode/sacc"
    },
    "RequestId": "2A3ABD81-95F5-4931-ACB3-31BDAE561FC7",
    "Success": true,
    "ErrorCode": 200
}
```
