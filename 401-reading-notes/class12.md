# Pandas in 10

Object creation¶

Creating a Series by passing a list of values, letting pandas create a default integer index:

`In [3]: s = pd.Series([1, 3, 5, np.nan, 6, 8])`

```In [4]: s
Out[4]: 
0    1.0
1    3.0
2    5.0
3    NaN
4    6.0
5    8.0
dtype: float64```

Viewing data¶


Here is how to view the top and bottom rows of the frame:

`df.head()`
`Out[13]: `
                   A         B         C         D
`2013-01-01  0.469112 -0.282863 -1.509059 -1.135632`
`2013-01-02  1.212112 -0.173215  0.119209 -1.044236`
`2013-01-03 -0.861849 -2.104569 -0.494929  1.071804`
`2013-01-04  0.721555 -0.706771 -1.039575  0.271860`
`2013-01-05 -0.424972  0.567020  0.276232 -1.087401`

`df.tail(3)`
`Out[14]: `
                   `A         B         C         D`
`2013-01-04  0.721555 -0.706771 -1.039575  0.271860`
`2013-01-05 -0.424972  0.567020  0.276232 -1.087401`
`2013-01-06 -0.673690  0.113648 -1.478427  0.524988`


Selection

While standard Python / NumPy expressions for selecting and setting are intuitive and come in handy for interactive work, for production code, we recommend the optimized pandas data access methods, .at, .iat, .loc and .iloc.

Getting

df["A"]
Out[23]:
2013-01-01    0.469112
2013-01-02    1.212112
2013-01-03   -0.861849
2013-01-04    0.721555
2013-01-05   -0.424972
2013-01-06   -0.673690
Freq: D, Name: A, dtype: float64

Selection by label

 df.loc[dates[0]]
Out[26]: 
A    0.469112
B   -0.282863
C   -1.509059
D   -1.135632
Name: 2013-01-01 00:00:00, dtype: float64 

Selecting on a multi-axis by label:

```df.loc[:, ["A", "B"]]
Out[27]: 
                   A         B
2013-01-01  0.469112 -0.282863
2013-01-02  1.212112 -0.173215
2013-01-03 -0.861849 -2.104569
2013-01-04  0.721555 -0.706771
2013-01-05 -0.424972  0.567020
2013-01-06 -0.673690  0.113648 ```

Selection by position

df.iloc[3]
Out[32]: 
A    0.721555
B   -0.706771
C   -1.039575
D    0.271860
Name: 2013-01-04 00:00:00, dtype: float64


Boolean indexing

df[df["A"] > 0]
Out[39]: 
                   A         B         C         D
2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
2013-01-02  1.212112 -0.173215  0.119209 -1.044236
2013-01-04  0.721555 -0.706771 -1.039575  0.271860

Setting

Setting a new column automatically aligns the data by the indexes:

s1 = pd.Series([1, 2, 3, 4, 5, 6], index=pd.date_range("20130102", periods=6))

s1
Out[46]: 
2013-01-02    1
2013-01-03    2
2013-01-04    3
2013-01-05    4
2013-01-06    5
2013-01-07    6
Freq: D, dtype: int64

df["F"] = s1

notes taken from (https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)