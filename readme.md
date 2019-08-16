# REDAN Exchange API- Endpoints

* [Trading Pairs](#trading-pairs)
* [Ticker](#ticker)
* [24 Hr Volume](#24-hr-volume)
* [Order Book](#order-book)
* [Trade History](#trade-history)
* [Tokens & Pairs](#token-pairs)

## Trading Pairs

* **URL:**  https://www.redanexchange.com/market/API
* **Method:**  `GET /api/getpairs`
*  **URL Params:**  `None`
* **Success Response:** 
```
{  
    "status":"200",
    "message":"success",
    "pairs":[  
        "ETH_AOA",
        "ETH_EGT",
        "ETH_HT",
        "ETH_INO",
        "ETH_LEO",
        "ETH_LINK",
        "ETH_MKR",
        "ETH_NPXS",
        "ETH_RDAN",
        "ETH_TUSD",
        "ETH_VEN"
    ]
}
```

## Ticker

* **URL:**  https://www.redanexchange.com/market/API
* **Method:**  `GET api/ticker/[token]`
*  **URL Params:**   [`token`](#token)
* **Success Response:** 

Example: https://www.redanexchange.com/market/API/api/ticker/AOA

```
{  
   "status":"200",
   "message":"Success",
   "item":[  
      [  
         "1564398008",
         "0.00010759",
         "0.00000000",
         "0.00000000",
         "0.00010759",
         "7300.00000000"
      ],
      [  
         "1564397987",
         "0.00010770",
         "0.00000000",
         "0.00000000",
         "0.00010770",
         "7700.00000000"
      ]
   ]
}
```

## 24 Hr Volume

* **URL:**  https://www.redanexchange.com/market/API
* **Method:**  `GET /api/volume24`
*  **URL Params:**  `None`
* **Success Response:** 
```
{  
    "status":"200",
    "message":"success",
    "pairs":[  
        "ETH_AOA",
        "ETH_EGT",
        "ETH_HT",
        "ETH_INO",
        "ETH_LEO",
        "ETH_LINK",
        "ETH_MKR",
        "ETH_NPXS",
        "ETH_RDAN",
        "ETH_TUSD",
        "ETH_VEN"
    ]
}
```

## Order Book

* **URL:**  https://www.redanexchange.com/market/API
* **Method:**  `GET /api/orderbook/[token]`
*  **URL Params:**  [`token`](#token)
* **Success Response:** 

Example: https://www.redanexchange.com/market/API/api/orderbook/AOA

```
{  
   "status":"200",
   "message":"success",
   "buy":[  
      {  
         "date":"26-7-2019",
         "buycoin":"ETH",
         "sellcoin":"AOA",
         "refno":"1564149964",
         "orderrate":"0.0001342",
         "quantity":"25000",
         "total":"3.355"
      },
      {  
         "date":"26-7-2019",
         "buycoin":"ETH",
         "sellcoin":"AOA",
         "refno":"1564151150",
         "orderrate":"0.000108",
         "quantity":"10200",
         "total":"1.1016"
      },
      {  
         "date":"29-7-2019",
         "buycoin":"ETH",
         "sellcoin":"AOA",
         "refno":"1564395849",
         "orderrate":"0.00010796",
         "quantity":"9115",
         "total":"0.9840554"
      }
   ]
}
```

## Trade History

* **URL:**  https://www.redanexchange.com/market/API
* **Method:**  `GET /api/tradehistory/[token]`
*  **URL Params:**  [`token`](#token)
* **Success Response:** 

Example: https://www.redanexchange.com/market/API/api/tradehistory/AOA

```
{  
   "status":"200",
   "message":"success",
   "pairs":[  
      {  
         "date":"29-7-2019",
         "tradetype":"BUY",
         "price":"0.00010759",
         "quantity":"7,300.00000000"
      },
      {  
         "date":"29-7-2019",
         "tradetype":"BUY",
         "price":"0.00010770",
         "quantity":"7,700.00000000"
      },
      {  
         "date":"29-7-2019",
         "tradetype":"BUY",
         "price":"0.00010732",
         "quantity":"4,137.00000000"
      }
   ]
}
```

## Tokens & Pairs

| #  | Token | Pairs |
| --- | --- | --- |
| 1  | AOA  | ETH_AOA  |
| 2  | EGT  | ETH_EGT  |
| 3  | HT   | ETH_HT   |
| 4  | INO  | ETH_INO  |
| 5  | LEO  | ETH_LEO  |
| 6  | LINK | ETH_LINK |
| 7  | MKR  | ETH_MKR  |
| 8  | NPXS | ETH_NPXS |
| 9  | RDAN | ETH_RDAN |
| 10 | TUSD | ETH_TUSD |
| 11 | VEN  | ETH_VEN  |
