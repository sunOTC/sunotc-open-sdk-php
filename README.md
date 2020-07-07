# SunOTC-open-sdk-php
>基于PHP的OTC商户api接口SDK

-------
### 安装方法

```
$ composer require sun-otc-open-sdk/sun-otc 
```

### 使用方法

```
use SunOTC\OTCService;

    $data       = '{"app_id":"123","merc_order_id":"200611184930170114"}';
    $OtcService = (new OTCService('', Dictionary::PRI_KEY));
    $OtcService->getOrderMsg($data);
    //                //查询交易限制
    $data       = '{"app_id":"123"}';
    $OtcService = (new OTCService('', Dictionary::PRI_KEY));
    $OtcService->getTradeLimit($data);*/
    
    //查询商户资产
     $data = '{"app_id":"123","merc_order_id":"200611184930170114"}';
     $OtcService = (new OTCService('',Dictionary::PRI_KEY));
     $OtcService->getMercAsset($data);
    
    //        //查询价格
    $data       = '{"app_id":"123","coin":"USDT"}';
    $OtcService = (new OTCService('', Dictionary::PRI_KEY));
    $OtcService->getTradePrice($data);
        
        
//返回数据
$address_info  = '{
                      "code":0,
                      "message":"success",
                      "data":[
                          {
                              "pay_type":"BANK",
                              "amount_min":1000,
                              "amount_max":5000
                          },
                          {
                              "pay_type":"WECHAT",
                              "amount_min":1000,
                              "amount_max":5000
                          },
                          {
                              "pay_type":"ALIPAY  ",
                              "amount_min":1000,
                              "amount_max":5000
                          }
                      ],
                      "time":1592729822
                  }'；
```

### 链接
* 




