# Adding new token
The JSON schema for the tokens includes: address, name, decimals, symbol, logoURI, official homepage, MarketCap link, existing Markets.

Follow the steps below to add a new token：
1) Fork this repo.
2) change the JSON file `tokenlist.json`, adding such as: (PLEASE DO NOT REMOVE EXISITING TOKENS)
```
{
      "address": "TH3KQd3Y8YE6WaBSgVd4sre9E8JTw99999",
      "symbol": "Timibbs",
      "name": "TimibbsTRC20",
      "decimals": 6,
      "logoURI": "(https://apilist.tronscanapi.com/api/top10?type=0&time=1)",
      "homepage": "(https://apilist.tronscanapi.com)",
      "MarketCapLink": "(https://apilist.tronscanapi.com/currencies/wink/)",
      "existingMarkets": [
          {
              "source": "Binance",
              "pairs": [
                  "Timibbs/USDT",
                  "Timibbs/BUSD",
                  "Timibbs/BNB",
                  "Timibbs/USDC"
              ]
          },
          {
              "source": "Poloniex",
              "pairs": [
                  "Timibbs/USDT"
              ]
          },
          {
              "source": "KuCoin",
              "pairs": [
                  "Timibbs/USDT"
              ]
          }
    ]
}
```
* `address`[Required]: your token address.
* `symbol`[Required]: your token symbol.
* `name`[Required]: your token name.
* `logoURI`[Required]: the logo URI of your token.
* `homepage`[Required]: the home page of your token.
* `MarketCapLink`[Optional]: the coinmarketcap or coingecko link for your token.
* `existingMarkets`[Required]: where to trade with your token.
3) Submit PR with the changed JSON file.


