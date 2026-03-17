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

