#[Cleaning log.txt](https://github.com/user-attachments/files/33303818/Cleaning.log.txt)
[Cleaning log.docx](https://github.com/user-attachments/files/33303826/Cleaning.log.docx)

## Data Dictionary

| Variable Name | Data Type | Unit | Definition | Source | Limitations |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `Effective_Date` | `datetime64[ns]` | Date | Official date on which the notified price takes effect | PSO / OGRA | Irregular gap of 13–16 days depending on month length |
| `Product` | `string` | Categorical | Commercial fuel category name (`PREMIER EURO 5`) | PSO Archives | Covers motor gasoline only; excludes high-speed diesel |
| `Price_PKR_L` | `float64` | PKR/Litre | Consumer retail price notified by the government | OGRA / PSO Notifications | Excludes regional dealer commission variations |
| `Brent_Crude_USD` | `float64` | USD/barrel | Global benchmark crude oil close price | Yahoo Finance (`BZ=F`) | Trading pauses on weekends and international holidays |
| `USD_PKR_Rate` | `float64` | PKR/USD | Official interbank/forex close exchange rate | Yahoo Finance (`PKR=X`) | Daily closing rate may differ from exact OGRA conversion rate |
