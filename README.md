# Stock Analysis
Module 2 Challenge

## Overview of Project
In order to diversify an investment portfolio, the client requested a deliverable which would analyze the performance of twelve green energy company stocks over the years 2017 and 2018. The client, an investment advisor, is particularly interested in analyzing how a particular stock, DQ, performs when comparted to similar companies. The deliverable will provide the total daily volume and percentage of return for each of the twelve selected stocks for the requested time period. 


## Results
The client provided two years of stock data for twelve green energy companies and requested a macro code be created in Excel in order to analyze their performance. The intention was to make the codes performance was fast and user friendly as possible, requiring the client to simple press a button on the spreedsheet and pick the year for the code to analyze. 

<img width="726" alt="Screen Shot 2021-05-07 at 9 23 37 PM" src="https://user-images.githubusercontent.com/82982901/117521230-b3a8ff00-af7a-11eb-8ca4-1d63e6b0b41b.png">

After writing the code to set the formatting for the All Stocks Analysis output sheet, the first in the analysis was to define the tickers variable and array of the twelve stocks with provided data. This ticker array and tickerIndex variable will provide the backbone for the rest of the code.

<img width="573" alt="Screen Shot 2021-05-07 at 9 28 48 PM" src="https://user-images.githubusercontent.com/82982901/117521362-5c575e80-af7b-11eb-8908-6671fde36718.png">

The next step was to define the tickersVolume, tickerStartingPrice, and tickerEndingPrice variables which will be part of the output on the All Stocks Analysis for the client. Using a for loop with nested conditionals, shown below, the tickerIndex will loop through the rows to determine the volume and find the starting and ending prices of the current ticker before repeating the process for each of the twelve tickers in the array.

<img width="626" alt="Screen Shot 2021-05-07 at 9 32 43 PM" src="https://user-images.githubusercontent.com/82982901/117521593-937a3f80-af7c-11eb-8adc-b9d2d9575116.png">

Once all twelve tickers have been looped through, the code will output the results of the analysis onto the spreadsheet for the client's review.

<img width="587" alt="Screen Shot 2021-05-07 at 9 39 39 PM" src="https://user-images.githubusercontent.com/82982901/117521692-156a6880-af7d-11eb-8e5d-68a0946e0159.png">

Using this output, we are able to determine only two stocks in the data set achieve positive returns in both 2017 and 2018, ENPH and RUN.

<img width="567" alt="Refactored 2017 Output" src="https://user-images.githubusercontent.com/82982901/117521834-e6a0c200-af7d-11eb-8913-658f973a5883.png">

<img width="590" alt="Refactored 2018 Output" src="https://user-images.githubusercontent.com/82982901/117521839-e99bb280-af7d-11eb-8598-a66a67fd7a42.png">

Based on this analysis, I would recommend these two stocks, not the DQ stock, for investment.

The final step of the code, stops the timer we set to determine the speed with which the macro performs it's analysis.

<img width="616" alt="Screen Shot 2021-05-07 at 9 40 19 PM" src="https://user-images.githubusercontent.com/82982901/117521724-3e8af900-af7d-11eb-8956-7aa18cdd4e36.png">

The timer was critical to determining which of the two codes written as part of this deliverable were the most efficient and should be given to the client. In this case, the refactored code ran in .109 seconds which was a .5 seconds faster than the original code at .617 seconds for the 2017 data.

<img width="366" alt="Original 2017 Run Time" src="https://user-images.githubusercontent.com/82982901/117522106-8743b180-af7f-11eb-9b77-d00186c24583.png">

<img width="211" alt="Refactored 2017 Run Time" src="https://user-images.githubusercontent.com/82982901/117522109-8b6fcf00-af7f-11eb-8ab3-4128f3272924.png">

This was also true for the 2018 data with the refactored code running in .117 seconds and the original in .648 seconds.

<img width="272" alt="Refactored 2018 Run Time" src="https://user-images.githubusercontent.com/82982901/117522170-cf62d400-af7f-11eb-822f-050c3536c2cd.png">

<img width="211" alt="Refactored 2017 Run Time" src="https://user-images.githubusercontent.com/82982901/117522175-d2f65b00-af7f-11eb-9621-e883640e10a0.png">


## Summary
The refactoring code is one of the foundations of data analysis. The end goal of any code is to quickly and efficiently analyze data, refactoring code allows one to re-exam written code and finds ways to improve the pattern to increase efficiency. In the case of the data set analyzed in this deliverable, refactoring the code allowed us to decrease the run time of the macro by .5 seconds.

It can be difficult to refactor code when the original code does not contain comments to indicate the thought process of the code's writer. While code should follow logical processes and be easy to read, this is not always the case and the lack of comments can provide a stumbling block when one is refactoring unfamiliar code.
