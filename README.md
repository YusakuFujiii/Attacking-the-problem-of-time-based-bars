# Unstructured Data Processing
Here is a collection of implementation to derive a structured data set from the unstructured one.  

From Advances in Financial Machine Learning :  
- Sampling dollar bars from time bars
- Extracting relevant samples using the symmetric CUSUM Filter
  - We sample only when a cumulative absolute return exceeds a threshold.
  - This method is effective in reducing the amount of data and extracting meaningful information. 

Ideas for further research : 
- Sampling dollar bars where the size of the bar is dynamically adjusted as a function of something. 
