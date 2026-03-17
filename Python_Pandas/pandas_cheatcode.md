# Python Pandas Guide

### Importing 
import pandas as pd

### Read Function
df = pd.read_csv(r"E:\cust_table.csv")
df

### Header Function
df = pd.read_csv(r"E:\cust_table.csv", header = None, names = ["test"])
df 

this line allows us to change the header mostly if theres no header for the table


