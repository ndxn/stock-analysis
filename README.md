# Stock Analysis
This analysis is provide of the historical performance of green energy stocks for Steve and his family trust. In order to make the VBA script more efficient and robust, the script has been refactored to take advantage of arrays.

The original work done within the module has been changed to subroutine  AllStocksAnalysisModWork() whereas the Module 2 challenge subroutine retains the original name AllStocksAnalysis(). <br/>

### Challenge

This new analsys provides the same effective outputs as the original AllStocksANalysis() script but does so by recording values into an array before outputting them, thus potentially making the script more robust for additional data and later refactoring.

The main data collection script remains the same, wherein the script matches the called variable, ticker, with the ticker name in the data and, when those match, values from the data are stored in the apprpriate array.

There are two primary limitations with the script as it and both pertain to the ticker name array, with the result being that, if the stocks change, the script will be broken. The first is that the arrays are initiated at a specific length. If there are additional stocks added, the script itself must be changed. The second is similar in the ticker names are hard coded. A more robust script would search for and count the names with the data, establish a variable that stores the number of ticker symbols, create appropriately sized arrays, and then popublate the ticker array with the ticker names. A smaller drawback within the code is the reducance of the tickerIndex variable which is set to be the same as the loop iterators.

Final analysis is output from the array, with the year-end return being calculated at the time of output. <br/><br/>

#### Limitations and Conclusions from the Data

In order to get the most out of this tool, Steve is going to need to more data than he provided. If the additional years of data are for the same stocks, he will be able to run the script with no problem. However, two years of market data is not enough to establish trends.

What can be taken away from the analysis is that the stocks have performed moderately well. During 2017, most stocks were up and were so considerably--in a range from 5.5% to almost doubling in value. In 2018, stocks were down though, for the most part, not enough to erase the gains from 2017.

The year-end returns, while helpful in assessing stock performance, are not all that robust of indicators. Especially with energy stocks, it would be important to overlay perforamnce with energy market events in order to determine how resilient of performers the stocks are.
