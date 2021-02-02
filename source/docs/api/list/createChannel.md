# 创建通道

请求地址
--------------------------------------------------------------------------
POST /api/v1/namespaces/{namespace}/channel/

请求参数
---------------------------------------------------------------------------

| 名称 | 类型 |必填| 描述|示例值|
|-----|---  |---|----|---|
| token |String |是 |token| 30b1841b67f005189e0a3600f701a9f192df23e2|
| consortiumId |String |是 |组织ID| org-asiainfo|
| channelName |String |是 |通道ID| channel-asiainfo-union-1w55v3u39x2xz|
| batchTimeout |Integer |否 |块超时时间(S)| 2|
| maxMessageCount |Integer |否 |块交易上限| 50|
| preferredMaxBytes |Integer |否 |块大小软限制| 20|
| organizations |Object[] |是 |组织| 20|

### organizations 请求示例
```
{        
    "organizations":[
      {
          "orgId":"asiainfo-akpcsjjac2jd",
          "peerId":"asiainfo-peer-kkpcsjsfc5ty",   
          "type":"commit"
      }
    ]  
}
```


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
    "Result":[
      {
          "ChannelId":"chan-channelx-1l1hmckuuisxo",
          "ConsortiumName":"aaaaa",   
          "ChannelName":"channelx",
          "ConsortiumId":"consortium-aaaaaa-akpcsjjac2jd",
          "CreateTime":"1544768139624",
          "MaxMessageCount":50,
          "MemberCount":2,
          "OwnerBid":"26842",
          "OwnerUid":"",
          "OwnerName":"name",
          "PreferredMaxBytes":12,
          "State":"Pending",
          "SupportConfig":"true",
          "UpdateTime":"1544768139624"
          }
    ],   
    "RequestId":"",
    "Success":true,
    "ErrorCode":200   
}
```