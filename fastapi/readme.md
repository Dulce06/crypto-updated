pip install fastapi
pip install "uvicorn[standard]"

uvicorn messari:app --reload

 
Function 1: 
For a given date, given crypto currency name, given moving average - calculate the moving average 
and return symbol, name, moving average, date.

http://127.0.0.1:8000/f1?before=2022-03-16&limit=01&name=btc


Function 2:
Calculate 50 moving average and 20 moving average first.
If 20 moving average is greater than 50 moving average - it’s bullish 
If 20 moving average is less than 50 moving average  - it’s bearish 

http://127.0.0.1:8000/f2?name=btc

Function 3: 
Confirming if we should buy or sell the stock
Buy if : 
20 moving average greater than 50 moving average
Current price is above 20 and 50 moving averages
The current volume is greater than yesterdays volume
Esle sell 

http://127.0.0.1:8000/f3?name=btc