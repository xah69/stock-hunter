# stock-hunter
stock-hunter is a command line tool for calculating the indicators(RSI,BB,MACD,EMA,EMAC) and providing the signals and recomendation of one or more than one stocks that you put in config file.

[Note]
* It supports intraday as well as positional time period
* It works in linux os only
* It provide support for only Indian Stocks(NSE)

[Installation and configuration]
1. extract the zip file 
2. cd into the folder extracted
3. execute $ chmod +x dependencies.sh
4. execute $ ./dependencies.sh
5. for intraday stocks : open config.py from path--> <user>/pha folder and put the NSE stock symbols you want inside the pairs array
6. 5. for positional stocks : open config.py from path--> <user>/pha/mew folder and put the NSE stock symbols you want inside the pairs array

[Usage]
1. $ cd <user>/pha
2. $ python3 tokling.py
3. you will have to choose one option either "i" for intraday or "p" for positional

(Intraday) : 
1. first u have to give the date from which you want to start like this
> [enter starting date] --$ 1/1/2023
3. then u have to give the time period either (1,3,5,15,60) in minutes like this
> [enter time period  ] --$  15

*output will be like this*
+-----------+-----------+-----------+---------+----------+
|   stock   |    rsi    |     bb    |   macd  |   ema    |
+-----------+-----------+-----------+---------+----------+
|    INFY   |  oversold |  weak buy | bullish | down 1+% |
| TATASTEEL | no signal | no signal | bearish |   down   |
|   DABUR   |  oversold | no signal | bearish | down 1+% |
+-----------+-----------+-----------+---------+----------+


(Positional)
1. first u have to give the date from which you want to start like this
> [enter starting date] --$ 1/1/2023
3. then u have to give the time period either (1d,1w,1m) in day,week,month like this
> [enter time period  ] --$  1d

output will be like this
+------------+-----------+------------+---------+---------------+---------+
|   stock    |    rsi    |     bb     |   macd  |      ema      |   emac  |
+------------+-----------+------------+---------+---------------+---------+
|    ITC     | no signal | no signal  | bearish | nearby middle | bullish |
| HINDUNILVR | no signal | no signal  | bearish |    down 1+%   | bullish |
| NESTLEIND  | no signal | no signal  | bearish |    down 1+%   | bullish |
| TATACONSUM | no signal | no signal  | bearish |    down 1+%   | bullish |
| BRITANNIA  | no signal | no signal  | bearish |    down 1+%   | bullish |
| GODREJIND  | no signal | no signal  | bearish |    down 1+%   | bearish |
|   DABUR    | no signal | no signal  | bearish |       up      | bullish |
|   MARICO   | no signal | no signal  | bearish |       up      | bearish |
| MCDOWELL-N |  oversold | no signal  | bearish |    down 1+%   | bullish |
|   AMBER    | no signal | no signal  | bearish |       up      | bearish |
| BATAINDIA  | no signal | no signal  | bullish |    down 1+%   | bearish |
| BLUESTARCO | no signal | no signal  | bearish |    down 1+%   | bullish |
|  CROMPTON  | no signal | no signal  | bullish |    down 1+%   | bearish |
|   DIXON    | no signal | no signal  | bullish |    down 1+%   | bearish |
|  HAVELLS   | no signal | no signal  | bullish |     up 1+%    | bearish |
| KAJARIACER | no signal | overbought | bullish |     up 1+%    | bullish |
| ORIENTELEC | no signal | no signal  | bearish | nearby middle | bearish |
| RAJESHEXPO | no signal | no signal  | bullish |     up 1+%    | bullish |
|   RELAXO   | no signal | no signal  | bearish |    down 1+%   | bearish |
| TTKPRESTIG | no signal | no signal  | bullish |    down 1+%   | bearish |
|   TITAN    | no signal | no signal  | bullish | nearby middle | bullish |
|   VGUARD   | no signal | no signal  | bearish |      down     | bullish |
|   VOLTAS   | no signal | no signal  | bullish | nearby middle | bearish |
| WHIRLPOOL  | no signal | no signal  | bullish |       up      | bearish |
| ABBOTINDIA | no signal | no signal  |   buy   |     up 1+%    | bullish |
+-------------------------------------------------------------------------+

[additional command]
you use --> "c" for clearing the output
            "q" for quiting or exiting 

