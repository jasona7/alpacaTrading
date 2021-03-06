<h1 align="center">Welcome to alpacaTrading 👋</h1>
<h2 align="center">Automated Alpaca Trading API Order entry</h2>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0-blue.svg?cacheSeconds=2592000" />
</p>

> Python bracket order for alpaca order api

![Screenshot](python-aws-alpaca.png)

## Requirements
* Python 3.6 or higher
* [AWS Chalice](https://github.com/aws/chalice)
* [TradingView PRO](https://www.tradingview.com)

## Usage

**app.py**
Edit the limit_price and stop_price variabes to set a gain/loss limit for orders (ex. below 5% gain, and 2% stop loss)
```
"take_profit": {
            "limit_price": webhook_message['close'] * 1.05
        },
        "stop_loss": {
            "stop_price": webhook_message['close'] * 0.98,
        }
```

**TradingView Alert JSON BODY**
```
{
    "open": {{open}},
    "high": {{high}},
    "low": {{low}},
    "close": {{close}},
    "exchange": "{{exchange}}",
    "ticker": "{{ticker}}",
    "volume": {{volume}},
    "time": "{{time}}",
    "timenow": "{{timenow}}"
}

```



## Author

👤 **Jason Alloway**

* Website: www.linkedin.com/in/jasonalloway
* Github: [@jasona7](https://github.com/jasona7)

## Show your support

PLZ give a ⭐️ if this code was helpful!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
