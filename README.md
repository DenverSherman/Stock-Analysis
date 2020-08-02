# Stock-Analysis
Diversifying within green energy

## Background
In uncovering a complete disregard for diversification in his parent's stock portfolio (100% investment in 'DQ'), Steve asked around for tools to help find promising stocks to diversify. A VBA project is created to facilitate this project, showing trading frequency and yearly return by ticker for green energy stocks, 2017 to 2018.

## Results
As in most investing, clients wish to see the highest return on investment. My analysis highlights three of the highest returning stocks from 2017 as ENPH, FSLR, and SEDG with 129.5%, 101.3% and 184.5% respectively. For 2018, only ENPH and RUN saw positive returns at 81.9% and 84.0% respectively. Forward looking, RUN is traded actively, trading volume increased 87.8% between 2017 and 2018. Daily trading volume is noted as a measure of price accuracy by Steve's parents, "They believe that if a stock is traded often, then the price will accurately reflect the value of the stock".

Shortly speaking, look towards **RUN** and **ENPH** to diversify your green energy portfolio as both increased return with increase pricing accuracy from 2017 to 2018.

## Technical Summary
Our program loops through all data points to find variable starting and ending prices, summing all day trade volumes in between. This is arranged in 4 arrays: tickers, tickerVolumes, tickerStartingPrices, and tickerEndingPrices. Each is assigned to an index (aptly names tickerIndex) which ranges 0 to 11 (one for each ticker). The processing timing is remarkably consistent, posting the exact same benchmark time forom initiation to formatting as seen in the followiung screenshots.

![VBA Challenge 2017](https://github.com/DenverSherman/Stock-Analysis/blob/master/Resources/VBA_Challenge_2017.png)

![VBA Challenge 2018](https://github.com/DenverSherman/Stock-Analysis/blob/master/Resources/VBA_Challenge_2018.png)

Through refactoring into arrays, we were able to save 10% of the processing time. In retrospect, this may have not been necessary for this particular data set (only saving .07 seconds) however, as the number of data points increases, refactoring becomes increasingly valuable. Since our code is built in a mostly general sense (automatic starting and ending prices yet each ticker in the tickers(12) array are named individually), our refactored code could save more time when the set is increased. Should Steve's parents look beyond investment into green energy (thus bringing more tickers into play), our program saves more time as dataset size increases.
