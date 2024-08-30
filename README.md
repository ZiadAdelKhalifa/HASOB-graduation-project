Steps of the project :

1- Data Analysis : analysis the data of UCI Heart Disease Data and clean 
to deal with null values i had two options one is to delete null but i saw that the data will be only 299 row from 920 total number so it is not a good decition
i used another ways to deal with it like median and mode
i used some function to understand the data like 
describtion and info value counts unique calues in each columns 
then i used the cleaned data to find the relations between the features in the data 
show some plots for individual columns and some between two columns and between all the columns



2- Model :Bukting the model for predection 
first clean the data like we did in Data analysis notebook and make some preprocessing like encodding , standerscaler ,splitting the data then 
building our model and show the performance of it
next stepp is to save the model ,encoder (onehot encoder and lable encoder )and stander scaler ,finally make an example of how to use the model and process the input to be
suitable  for my model and to get suitable output this step help me alot in the part of flask app so i already know in this step how to process the input from the user to be suitable for my model 
then do the predection and bring my result and show it 

3-app :flask code which we use to take inputs from the patients or from the doctor and make some processing in it then send it to our model to get the predection 
same processing was in the model notebook when show an example


4-templates:contain index.html 
using a basic html page called index.html to show some lables to write in the values of the feature and predict button and show the returned predection

saved files :
1-heart_disease_encoder.pkl :saving the label encoder
2-heart_disease_model.keras:saving my model
3-heart_disease_OneHotEncoder.pkl:saving the onehot encoder
4-heart_disease_standard_scaler.pkl:sasving stander scaler
5-heart_disease_uci:the csv file which contain the data
