# Stock-analysis
Performing the analysis on the green energy stocks using Visual Basic for Applications to help Steve know the stock market trends for the years 2017 and 2018.
 

## Overview of the Project
This analysis aims to help steve analyze the green energy stocks as their parents are interested in investing in DAQ0 stock. Before investing their money, they want steve to check the performance of the stocks over a few years.
### Purpose
This challenge aims to refactor the original VBA code developed for all stocks analysis as the execution time was more.
In order to proceed with the analysis, Steve wants to calculate the total daily volume and yearly returns for each stock. Daily volume is the total number of shares traded throughout the day, and it measures how actively a stock is traded. If a stock is traded often, then the price will accurately reflect the value of the stock. The yearly return is the percentage difference in price from the beginning to the end of the year.

## Results
### Running DQ Analysis
Using VBA, the code was initially developed to check the total volume and returns of the DQ stock. By seeing the return percentage, we can see that there was 200% increase in 2017 where as in 2018 it was 63% drop in the value for DQ stock.So it will not be wise decisionfor steve to suggest his parents invest in DQ stock.Inorder to find a better option, he analyzed the multiple stocks.

![image](StockAnalysis_output/DAQO.png)

### Running All the Stocks Analysis using Original code:
In order to run the analysis on all the stocks, we need to create an array list for stocks named tickers; using nested for loops, we need to calculate the volumes and returns for each ticker. For the outer loop, we use the index of the ticker, and for the inner loop, we iterate from starting of the row to last row of the worksheet, so for each ticker, the code has to run through the entire worksheet, which increases the run time of the code.

### Comparing 2017 and 2018 Stock Analysis Data
Based on the results of the analysis of the stocks categories we can see that 2017 has successful return as 11 out of 12 major stocks has positive returns where as in 2018 we can see only 2 out of the 12 stocks has positive returns.So more people would have been profited in 2017.The below screenshots shows the run time for both the years using original code.

| 2017          | 2018          |
| ------------- | ------------- |   
|<img src = "StockAnalysis_output/AllStocksAnalysis2017.png" width = "350">| <img src = "StockAnalysis_output/AllStocksAnalysis2018.png" width = "350"> |
|<img src = "StockAnalysis_output/Performance_AllStockAnalysis2017.png" width = "400">| <img src = "StockAnalysis_output/Performance_AllStockAnalysis2018.png" width = "400"> |

### Running All the Stocks Analysis using refactor code:
In the refactor code we have used three output arrays such as total volume,total starting price,total ending price and we have used tickerindex which runs through the entire worksheet.Here we have used only one for loop to calculate the total volume and returns.We print the value in the worksheet using seperate for loop.so the code takes less memory and it is more efficient.

| Original code         | Refactored code         |
| -------------         | -------------           |
|![image](StockAnalysis_output/OriginalCode.png) | ![image](StockAnalysis_output/RefactoredCode.png)  |
                        
The results of the analysis of the stocks using original code and the refactored are the same but the run time is reduced in the refactored code.
we can say that the run time is improved 5 times the original code.

| 2017          | 2018          |
| ------------- | ------------- |
| ![image](StockAnalysis_output/VBA_Challenge_RefactorCode_2017.png) | ![image](StockAnalysis_output/VBA_Challenge_RefactorCode_2018.png)  |
|![image](Resources/VBA_Challenge_2017.png)                          | ![image](Resources/VBA_Challenge_2018.png) |

In this analysis,the values are color coded using static and conditional formatting.The green indicates the positive returns and where as red indicates the negative returns.

## Summary
### Advantages and Disadvantages of refactoring code in general
- Refactoring makes to improve the design,performance efficiency,readabililty of the existing code with out adding extra functionality.
- It makes the code more readable and maintainable and reduces the complexity.
- It makes runtime faster and it is helpful when we are dealing with large amount of data.
- The disadvantage of refactoring is some times the code may change the data and it may introduce errors in the code.
- Sometimes it may be time consuming if the code is not commented and explained properly.

### Advantages and disadvantages of the original and refactored VBA script
- In our VBA Script,the refactored code runs 5 times faster than the original which improves the efficiency of the code.
- It avoids nested for loops so we no need to switch back and forth the worksheet,It used single variable to access all the data from the worksheet and stores all the output data in arrays,which is printed seperately.
- The original code worked well for less number of data set but when we have large number of dataset like thousands of stocks it takes more time.
so the refactored code works more efficiently.
- There are no noticeable disadvantage of the refactored script,it just takes some time to make the original script run correctly with out errors,But its worth since we made an efficient code. 





















