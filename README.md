# Module-2-Challenge
## Challenge Overview
The purpose of this project was to refactor code to allow for a faster analysis of a series of stocks for our client, Steve, so that he could potentially analyze thousands instead of just a few dozen. To optimize the code, we used arrays and indexes to allow the code to run faster by reading a stored variable, instead of looping through more data for each item.

## Results
We refactored the central portion of the code, which describes which parts of the data to loop over, and what to do with that data. First, we had to create the actual tickerIndex variable, that would store our various ticker values. Since the ticker is a group of letters, we define the variable as a string

![Screen Shot 2022-09-22 at 3 19 26 PM](https://user-images.githubusercontent.com/112847821/191861325-9e1e7819-9882-4eb5-9fa5-2b9cd3ee75b4.png)

From here, we want to create out output arrays with space for all 12 ticker values.

![Screen Shot 2022-09-22 at 3 22 31 PM](https://user-images.githubusercontent.com/112847821/191861714-fdb93164-c4c9-4931-adfa-6d3e6d1d3080.png)

Next, we'll create our loops:

![Screen Shot 2022-09-22 at 3 23 24 PM](https://user-images.githubusercontent.com/112847821/191861809-5eb9859a-0f5d-4127-a13d-b1d6776d9c32.png)

Within these, we first initialize the tickerVolumes variable, which will return the volume for each ticker, as 0, so that it can increase per each ticker and reset when it moves to the next ticker loop. Finally, we can output our data. We then tell our code to start counting tickerVolumes for the first ticker stored within the tickerIndex. Then, the starting and ending price arrays are also assigned values, based on that first loop. Onces this is complete for all values in a ticker, the tickerIndex will increase. 


Finally, we can output our findings with the following code:

![Screen Shot 2022-09-22 at 3 26 02 PM](https://user-images.githubusercontent.com/112847821/191862116-0871d3ce-2322-4bde-807f-1d7a54099918.png)

As we can see, this new set of loops and arrays within our code allows the program to process much quicker. For 2018, the difference between the old (unrefactored, left) and new code (refactored, right) can be seen in that the new code on the right runs faster. 

![Screen Shot 2022-09-22 at 3 29 01 PM](https://user-images.githubusercontent.com/112847821/191862477-f026d37b-2688-4ff0-84b9-d92885c59e6b.png)
![Screen Shot 2022-09-22 at 2 59 55 PM](https://user-images.githubusercontent.com/112847821/191862309-5844fde9-ca46-423a-9a81-95ca8fe62b18.png)


## Analysis

### Pros and Cons of Refactoring
The main advantage that we have in refactoring this code, is that we are able to get it to run faster. This isn't immediately apparent for the size of sample that we're working with in this case, as the difference is a few tenths of a second, but for data sets that have potentially thousands of ticker-like variables, this could potentially save hours. Additionally, refactoring allows us to start with a majority of code written out, allowing us to just have to make a few small changes to achieve our goals.
The disadvantage, however, is that you may take a code that works well, and introduce new bugs and errors into it within the refactored code, that will make it not work as well, or even at all. This was my biggest challenge with this project- my original code worked excellent, but when refactoring and troubleshooting my new code, the functionality was minimal at best for a period. Alternatively, refactoring could be disadvantageous if you're working from code that isn't well notated or explained- if you're unaware of how the code works in the first place, it will be very difficult to refactor it to work more efficiently. 
### Pros and Cons of Refactoring this Project
As stated previously, the main advantage is that this code now runs faster! Further, refactoring our original code allowed us to utilize the first code as a jumping off point to create a more complex VBA Macro that was more powerful. So in this case, along with speeding up our code, it also served to allow us to create a more sophisticated code than we would have to solve the initial set of problems we were presented. 
The disadvantage is that the improvement, while measurable, is minimal- a few tenths of a second off of a code that takes just over 1 second to run is not a major improvement. As a result, the time spent refactoring this code and the increased sophistication seems to have yielded a small reward compared to the effort applied. This being said, if Steve was to use this for further research and expand the number of stocks, this disadvantage would shrink quickly. 





