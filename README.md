# YahooFinance.NET
Download historical end of day stock data and historical dividend data via the Yahoo Finance API

Install via NUGET
```
Install-Package YahooFinance.NET
```

Usage
```csharp
using YahooFinance.NET;

string exchange = "ASX";
string stockCode "AFI";
string yahooStockCode = yahooFinance.GetYahooStockCode(exchange, symbol);

YahooFinanceClient yahooFinance = new YahooFinanceClient();
List<YahooHistoricalPriceData> yahooPriceHistory = yahooFinance.GetHistoricalPriceData(yahooStockCode);
List<YahooHistoricalDividendData> yahooDividendHistory = yahooFinance.GetHistoricalDividendData(yahooStockCode);
```
