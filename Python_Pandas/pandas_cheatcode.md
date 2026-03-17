# Python Pandas Guide

### Importing 
import pandas as pd

### Read Function
df = pd.read_csv(r"E:\cust_table.csv")
df

 this is better for reading csv file

df = pd.read_table(r"E:\cust_table.text")
df

  this is better for reading text file 

df = pd.read_json(r"E:\cust_table.json")
df

  this is better for reading json files

df = pd.read_excel(r"E:\cust_table.xlxs")
df

  this is better for reading excel files



### Header Function
<p> df = pd.read_csv(r"E:\cust_table.csv", header = None, names = ["test"] )
df </p> 

this line allows us to change the header mostly if theres no header for the table

### separator Function
df = pd.read_csv(r"E:\cust_table.text", sep = "\t")
df

df = pd.read_csv(r"E:\cust_table.text", sep = ",")
df

this separator function when we use diffrent read function with different extension name allow us to still able to read / arrange the table in better case 

### Sheet Reading Excel file

df = pd.read_excel(r"E:\Example Run(excel).xlsx", sheet_name = 'Example Run')
df 

we just need to specify which sheet name to show when a excel file consist a lot sheets

### Option Max column - max rows 


pd.set_option('display.max.rows', 10000)
pd.set_option('display.max.columns', 45)

   this line help us able to show how many range we want to see in columns and rows that makes the output viewable


### Data info Function

df2.info() - df2 = df or call out name of a line 

e.g df2 = pd.read_excel(r"E:\Example Run(excel).xlsx", sheet_name = 'Example Run')
df2

   this give us information about our data files 
   
### Data Size df.shape Function

df2.shape 

  this shows us the column and rows

### Data rows head Df.head Function 

df2.head(5) 

   this shows the first 5 rows 

### Data rows tail Df.tail Function

df2.tail(5)

 this shows the last 5 rows 

### Data select Function

 df2['fullname']

   this allows us to select which rows to show / display
   
### Data location Loc and iloc Function

df2.iloc[224]
df2.loc[df2['fullname'] == "Alina Osterloh"]

  this allow us to get specific information the one with integer can be use as iloc function
  2nd row allow us to find excact data when we know their name or clue to the specific data

df2.iloc[224]
df2.iloc[10:25, 0:2]

   this alows us to get data using rows index number
   this allow us to find data close to what we expect using ranges 


