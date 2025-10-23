# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
```
## Output
<img width="980" height="174" alt="image" src="https://github.com/user-attachments/assets/1127e27e-e8ef-4b77-970c-bd81d2db5609" />

```python
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot') 
```
## Output
<img width="450" height="383" alt="image" src="https://github.com/user-attachments/assets/c5a4862a-fe18-4d0e-92d5-80a4582dd6fc" />

```python
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
```
## Output
<img width="452" height="380" alt="image" src="https://github.com/user-attachments/assets/5be7fb26-5942-46ae-a483-7717efa57607" />

```python
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
```
## Output
<img width="583" height="410" alt="image" src="https://github.com/user-attachments/assets/9572e863-cf0f-436d-b34e-37766a5f9975" />

```python
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
```
## Output
<img width="485" height="390" alt="image" src="https://github.com/user-attachments/assets/1be446ab-a440-4e08-98ff-85c2a17df719" />

```python
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
```

## Output
<img width="483" height="385" alt="image" src="https://github.com/user-attachments/assets/f5b35252-972f-408a-bb9e-7c7ecc3aba19" />

```python
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```
## Output
<img width="484" height="382" alt="image" src="https://github.com/user-attachments/assets/4090ce58-32a2-4d74-9c33-8aa325f6dee9" />

```python
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
```
## Output
<img width="477" height="398" alt="image" src="https://github.com/user-attachments/assets/d6eccf83-554b-48b0-b68b-d60d65307fe5" />

```python
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
```
## Output
<img width="478" height="390" alt="image" src="https://github.com/user-attachments/assets/8b0fcaa2-bd8e-4131-9bf6-f814a2aadbbd" />

```python
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
```
## Output
<img width="502" height="398" alt="image" src="https://github.com/user-attachments/assets/a8f74dbe-8f1d-4838-960d-cb65076a7f83" />

```python
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```
## Output
<img width="505" height="430" alt="image" src="https://github.com/user-attachments/assets/e70e12d0-dec6-4607-a205-48ff5104001f" />

# Result:
 Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
