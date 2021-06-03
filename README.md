# Swop.fi
Json for swop.fi
## Pools DApp Address
1) USDN/USDT: 3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1
2) NSBT/USDN: 3P2V63Xd6BviDkeMzxhUw2SJyojByRz8a8m
3) WAVES/USDN: 3PHaNgomBkrvEL2QnuJarQVJa71wjw9qiqG
4) USDTLP/USDN: 3PDWi8hjQJjXhyTpeaiEYfFKWBd1iC4udfF
5) SWOP/USDN: 3P27S9V36kw2McjWRZ37AxTx8iwkd7HXw6W
6) BTC/USDN: 3PACj2DLTw3uUhsUmT98zHU5M4hPufbHKav
7) WAVES/BTC: 3P8FVZgAJUAq32UEZtTw84qS4zLqEREiEiP
8) USDC/USDN: 3PNi1BJendWYYe2CRnqpfLoYxUZ6UTcx3LF
9) WCT/USDN: 3PMDFxmG9uXAbuQgiNogZCBQASvCHt1Mdar
10) SIGN/USDN: 3P4Ftyud3U3xnuR8sTc1RvV4iQD62TcKndy

## Token ID's
1) sUSDT_USD-N:  BNQ8bxyiWvfHzHAtNyfc6E7v3sSHXKq8yuit6Fnz1A3Q
2) sNSBT_USD-N:  HWFcdC9wjPJY1udkR2UsfXzyPptzBb9m6df8qUW6LNLo
3) sWAVES_USD-N: Btw3G1j4wQgdp49PTxaFkNvn75dQtqGDM7ejQppHnWC1
4) sUSDLP_USD-N: 9Pm2c97VzGSK6p8XGMCFABs575K9Cb35GdKtzwVA59m9
5) sSWOP_USD-N: ESg4EvZaY74xe3p2dxHeXpV3RNeJd7fda4aN9RtL4bzn
6) sWBTC_USD-N: 58RNQJqLQ3tYYpkjuJujWzLzMX3nzpGn6bTC8LfLtgAM
7) sWAVES_WBTC: 2DiiWi3RLuTYBj81iwACCSayD9d1aY2ucfoJUBDHiqH8
8) sUSD Coi_USD-N: 6en9RSUmqsh5j9sYeWYUvPM2r8QXVcwscdJorgdF3uxH
9) sWavesCo_USD-N: AAmQ1M3pG9fP882RJdfeaoLbRtzBuwPmsximGhPXVQXN
10) sSIGN_USD-N: CQpTLSuvKBtFo9BX4jNPopFnqCbE4VsqTcZrAwBgTTt5
11) sTurtleN_USD-N: 4kZ5zLkGweMSQZcsbaS4DCNsP4G4YXryJrbekvz1zoAF

## Token Decimals
1) sUSDT_USD-N:  6 decimals
2) sNSBT_USD-N:  6 decimals
3) WAVES/USDN: 7 decimals
4) sUSDLP_USD-N: 6 decimals
5) sSWOP_USD-N: 7 decimals
6) sWBTC_USD-N: 7 decimals
7) sWAVES_WBTC: 8 decimals
8) sUSD Coi_USD-N: 6 decimals
9) sWavesCo_USD-N: 4 decimals
11) sTurtleN_USD-N: 7 decimals 

## Stake usdn/usdt token to farming pool

String value = dapp from pool

AssetId = assetId from pool token
```

{
  "type": 16,
  "version": 2,
  "dApp": "3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw",
  "call": {
    "args": [
      {
        "type": "string",
        "value": "3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1"
      }
    ],
    "function": "lockShareTokens"
  },
  "payment": [
    {
      "assetId": "BNQ8bxyiWvfHzHAtNyfc6E7v3sSHXKq8yuit6Fnz1A3Q",
      "amount": "1000000"
    }
  ],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87
}
```

## Unstake NSBT/USDN
String value = dapp from pool

```

{
    "type": 16,
    "version": 2,
    "dApp": "3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw",
    "call": {
        "args": [
            {
                "type": "string",
                "value": "3P2V63Xd6BviDkeMzxhUw2SJyojByRz8a8m"
            },
            {
                "type": "integer",
                "value": 1000000
            }
        ],
        "function": "withdrawShareTokens"
    },
    "payment": [],
    "fee": 500000,
    "feeAssetId": null,
    "chainId": 87
}
```

## Claim swop early bird

```
{
  "type": 16,
  "fee": 500000,
  "feeAssetId": null,
  "version": 2,
  "chainId": 87,
  "dApp": "3PJuspTjxHhEJQjMEmLM5upiGQYCtCi5LyD",
  "payment": [],
  "call": {
    "function": "claimSWOP",
    "args": []
  }
  }
  ```

## Claim normal swop
String Value = pool dapp address
  ```
{
  "type": 16,
  "version": 2,
  "dApp": "3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw",
  "call": {
    "args": [
      {
        "type": "string",
        "value": "3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1"
      }
    ],
    "function": "claim"
  },
  "payment": [],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87,
  "proofs": []
}
  ```
## Governance token stake /Lock swop
  ```
{
  "type": 16,
  "version": 2,
  "dApp": "3PLHVWCqA9DJPDbadUofTohnCULLauiDWhS",
  "call": {
    "args": [ ],
    "function": "lockSWOP"
  },
  "payment": [
    {
      "assetId": "Ehie5xYpeN8op1Cctc6aGUrqx8jq3jtf1DSjXDbfm7aT",
      "amount": "100000000"
    }
  ],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87
}
  ```
  
## Governance token wd
  ```
{
  "type": 16,
  "version": 2,
  "dApp": "3PLHVWCqA9DJPDbadUofTohnCULLauiDWhS",
  "call": {
    "args": [
      {
        "type": "integer",
        "value": 100000000
      }
    ],
    "function": "withdrawSWOP"
  },
  "payment": [],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87
}
  ```
  
## Governance reward claim
  ```
{
    "type": 16,
    "fee": 500000,
    "feeAssetId": null,
    "version": 2,
    "chainId": 87,
    "dApp": "3PLHVWCqA9DJPDbadUofTohnCULLauiDWhS",
    "payment": [],
    "call": {
        "function": "claimAndWithdrawSWOP",
        "args": []
    }
}
  ```
## Checking how many tokens are staked
The available amount for unstaking can be determined via the node API, by calling the following endpoint:
```
wget https://nodes.wavesexplorer.com/addresses/data/3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw/<pools-dapp-address>_<address-to-check>_share_tokens_locked
````
