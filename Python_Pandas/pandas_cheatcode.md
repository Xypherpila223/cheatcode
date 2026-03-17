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




