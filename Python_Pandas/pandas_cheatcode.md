# Python Pandas Guide

### Importing 
import pandas as pd

### Read Function
df = pd.read_csv(r"E:\cust_table.csv")
df

\\\ this is better for reading csv file

df = pd.read_table(r"E:\cust_table.text")
df

\\\

### Header Function
df = pd.read_csv(r"E:\cust_table.csv", header = None, names = ["test"])
df 

this line allows us to change the header mostly if theres no header for the table

### separator Function
df = pd.read_csv(r"E:\cust_table.text", sep = "\t")
df

this separator function when we use diffrent read function with different extension name allow us to still able to read / arrange the table in better case 
