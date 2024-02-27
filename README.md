This is a short summary of the work involved in this project. There are 3 parts to the Jupyter Notebook. The first part is all about getting familiar with the data and following the examples/questions proposed by the program. The second part is our own analysis of the data, in a different category. And the last part is the conclusion. 

There are a total of 16 files in this repository (1 readme.md; 1 jupyter notebook – module5_coupon_es.ipynb in the notebook folder and 14 images in the image folder)

Link to Notebook: https://github.com/sinclaireric77/module5/tree/main/notebook/module5_coupon_es.ipynb

1st part
First, I cleaned the data by removing the car column as it is mostly filled with null values. Then for the remaining columns that have null values, I replace those with the median. I had to do a little bit of conversion because I had to calculate the median based on strings and using the sort function would not work. The order of string in our case is "1-3", "4-8", "gt8", "less1", "never" but we really want the order to be "never", "less1", "1-3", "4-8", "gt8" to calculate the median. I created a function to do just that.
After I had a clean dataset, I proceeded to complete the exercises on the bar coupon data only. Results in the notebook.

2nd part
The second part consists of finding similar patterns in a different set of data. I picked the “carry away and take out” data as it seems to have the highest acceptance ratio 73.5%. I looked at various parameters and the ones that seem to have the most impact are listed in the conclusion.

3rd part – Conclusion
In conclusion, for the “carry away and take out” data, I found that the marital status (widowed) seems to be the biggest factor for accepting the coupon with an 84.6% acceptance rate. The 2PM (86.7%) and 6PM (82.5%) were next with the time-of-day factor with a combined rate of acceptance of 83.9%. 
Then the other factors were:
1-	Not going to work (77.3%)
2-	50+ (77.4%)

The final overall rate for a person 50+ of age, widowed, not on their way to work and receiving the coupon at 2PM or 6PM was a staggering 100% but with only 11 data points. If we remove the “widowed” component, we have 88 data points and an acceptance rate of 89.8% which is still high.


![final_combined](https://github.com/sinclaireric77/module5/assets/160784197/064f1444-ee47-44e4-8c97-b2e09add0b92)
