
# Day-6
Feature Engineering- Feature engineering is all about transforming raw data into useful features that help make better predictions with machine learning models. It’s a crucial step that can improve your models and make your data easier to understand.

techniques of feature engineering: 

Create( creating new column from existing one )

Transform(Sometimes data exists but in the wrong form)

Tranformation ways:

Square Root,Cube Root,Reciprocal,Normalization

Encode(Convert categorical (text) data into numerical values so machine learning models can process it.)

Scale(Adjust numerical values to a common range or scale to improve model performance.)

Bin(Group continuous numerical values into categories or intervals.)

Extract(Extract useful information from an existing feature, such as numbers or dates from text.)

Combine(Merge two or more features to create a new, more informative feature.)

I have my dataset in which i use create,encode and extract type of feature engineering  

I create or extract  age and category now columns are title,tye,genre,release year rating ,duration,country,duration_num ,age,category and always remeber that after using label encoder col becomes numeric or int 


# Day-7

PCA- principal comonent analysis it is used for dimensionality reduction it means the features that are not imortant we reduct that we identify only important 

why we reduct features ??

more computation

more memory 

slower training 

sometimes lower accuracy 

PCA always works in numerical tye of data 

we remove release year because age also gives us same type of data 

we remove category because it gives same data as duration_num


# Day-8
imbalance class - in categorial col we have multile values so if we have imbalnced data means one category has more values than other

example- the column that ML model predicts we check that type - movie or tv show labelencoder  0 or 1 tv show has values 1400 and movie has values 200 so it is imbalanced we have various balancing techniques 

