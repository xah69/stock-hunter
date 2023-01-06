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
6. for positional stocks : open config.py from path--> <user>/pha/mew folder and put the NSE stock symbols you want inside the pairs array

[Usage]
1. $ cd <user>/pha
2. $ python3 tokling.py
3. you will have to choose one option either "i" for intraday or "p" for positional

(Intraday) : 
1. first u have to give the date from which you want to start like this
> [enter starting date] --$ 1/1/2023
3. then u have to give the time period either (1,3,5,15,60) in minutes like this
> [enter time period  ] --$  15

(Positional)
1. first u have to give the date from which you want to start like this
> [enter starting date] --$ 1/1/2023
3. then u have to give the time period either (1d,1w,1m) in day,week,month like this
> [enter time period  ] --$  1d

[additional command]
you use --> "c" for clearing the output
            "q" for quiting or exiting 

