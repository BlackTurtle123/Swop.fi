# Swop.fi
Json for swop.fi
#Pools
1) USDN/USDT: 3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1

2) USDN/NSBT: 3P2V63Xd6BviDkeMzxhUw2SJyojByRz8a8m

#Stake usdn/usdt token to farming pool
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

#Unstake NSBT/USDN
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

#Claim swop early bird


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
