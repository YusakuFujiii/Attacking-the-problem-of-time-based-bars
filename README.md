# Attacking the problem of poor statistical properties in time-based bars 
### Problem setting 
The statistical properties of time-based bars are known to be poor. One of the inferiorities of them is the absence of return normality, which is against the assumption that ML algorithms have. Then, how can we make time-based bars more desirable for ML algorithms to work? 

###  Existing methods
1. Sampling dollar bars from time bars
   - We sample only when the dollar value of a trading volume exceeds a threshold.
   - This method solves the issue with volume bars that they do not account for a change in trading volume associated with         price change in an asset
2. Extracting relevant samples using the symmetric CUSUM Filter
   - We sample only when a cumulative absolute return exceeds a threshold.
   - This method is effective in reducing the amount of data and extracting meaningful information. 
   
### Discussion
- What about sampling dollar bars where the size of the bar is dynamically adjusted as a function of something?
- Does a ML model that has learned from dollar bars work well with time-based bars that are provided in real time by an exchange API? 
 - 
