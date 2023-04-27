# Neural_Network_Charity_Analysis
![image](https://user-images.githubusercontent.com/111661058/234169400-ea790b37-cfce-4dd6-82fe-0028a98376e6.png)
## Purpose
Using our knowledge of machine learning and neural networks, we will use the provided dataset to create a binary classifier that is capable of prediciting weather applicants will be successful or not.
## Results
Our given dataset
![image](https://user-images.githubusercontent.com/111661058/234170769-e89c04b2-d46f-4dbc-a92b-9240c0f5ed08.png)

### Data Preprocessing
  1) What variable(s) are considered the target(s) for your model?<BR>
      The target variable is the IS_SUCCESSFUL column.
      
  2) What variable(s) are considered to be the features for your model?<BR>
      All remaining variables that are not removed are to be considered  the features. 
      
  3) What variable(s) are neither targets nor features, and should be removed from the input data?<BR>
      To start, the EIN and NAME columns will be removed because they do not effect the target variable.
      
### Compiling, Training, and Evaluating the Model
  4) How many neurons, layers, and activation functions did you select for your neural network model, and why?<BR>
       We began with 80 neurons, 3 layers, two activation functions. Because you have to start somewhere.     
        
  5) Were you able to achieve the target model performance?<BR>
      Was not able to get the needle to move off the approx. 72% accuracy rating.  
      
  6) What steps did you take to try and increase model performance?<BR>
      We tried several different combinations to optimize the model.
        * 1st Optimization -- dropped INCOME_AMT_0 -- kept and saved
        * 2nd Optimization -- Kept the same amount of neurons but spread them over 4 layers
        * 3rd Optimization -- Upped neurons to 260 over 6 layers
        * 4th Optimization -- Used same set up as 1st Optimization -- changed epochs from 50 to 500 -- changed hidden layer activation to LeakyReLU

## Summary
  After several different models were tried the accuracy rating did not increase in any notable way. 
#### Recommendations
   * Recommended columns to remove
      * ASK_AMT
      * STATUS
      * SPECIAL_CONSIDERATIONS
      * INCOME_AMT-- 24388 enties are '0' out of 34299 enties -- did remove INCOME_AMT_0)
   * More playing with the activation functions is needed on future models. In my limited amount of time I was not able to play much with these.
   * I wouldn't touch the neurons or epochs until the two previous steps showed some promise.
