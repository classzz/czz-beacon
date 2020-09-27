# docs

## 获取灯塔信息列表

Request path: ```http://localhost:8080/czzinterfaces/getStateInfo```

interface name: getStateInfo

## 根据灯塔id获取灯塔信息

Request path: ```http://localhost:8080/czzinterfaces/getStateInfoById```

interface name: getStateInfoById

## 获取地址在某个灯塔下的兑换信息

Request path: ```http://localhost:8080/czzinterfaces/getAddressExchangeInfo```
interface name: getAddressExchangeInfo

### 获取灯塔的自由额度

Request path: ```http://localhost:8080/czzinterfaces/getBeaconFreeAsset```

interface name: getBeaconFreeAsset

Response:

```json
{
    "state" : 200,
    "version" : "v1.0",
    "data" : {
         "doge": 1, //数量
         "ltc":	1,
         "btc":	1,
         "bsv":	1,
         "bch":	1
        }
}
```

### 获取灯塔的可兑换余额

Request path: ```http://localhost:8080/czzinterfaces/getBeaconExchangeAsset```

interface name: getBeaconExchangeAsset

```
#### sample
Request:

GET ``http://localhost:8080/czzinterfaces/getBeaconExchangeAsset``

Response:
```json
{
    "state" : 200,
    "version" : "v1.0",
    "data" : 1
}
```



### 获取各币种的兑换比例

Request path: http://localhost:8080/czzinterfaces/getRateInfo

interface name: getRateInfo

```
#### sample
Request:

GET http://localhost:8080/czzinterfaces/getRateInfo

Response:
```json
{
    "state" : 200,
    "version" : "v1.0",
    "data" : {
      "DOGE_CZZ":1,
      "LTC_CZZ":1,
      "BTC_CZZ":1,
      "BCH_CZZ":1,
      "BSV_CZZ":1,
      "USDT_CZZ":1,
    }
}
```
