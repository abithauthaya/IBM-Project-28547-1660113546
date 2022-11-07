# IBM-Project-28547-1660113546
AI-powered Nutrition Analyzer for Fitness Enthusiasts
Basic Python
1. Split this string
s = "Hi there Sam!"
print(s.split())
['Hi', 'there', 'Sam!']
2. Use .format() to print the following string.
Output should be: The diameter of Earth is 12742 kilometers.
planet = "Earth"
diameter = 12742
a="The daimeter of {planet}is{diameter}kilometers"
print(a.format(planet="Earth",diameter=12742))
The daimeter of Earthis12742kilometers
3. In this nest dictionary grab the word "hello"
d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}
print(d)
{'k1': [1, 2, 3, {'tricky': ['oh', 'man', 'inception', {'target': [1, 2, 3, 'hello']}]}]}
Numpy
import numpy as np
b=np.zeros(10)*0
print(b)
[0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]
4.1 Create an array of 10 zeros?
4.2 Create an array of 10 fives?
import numpy as np
b=np.ones(10)*5
print(b)
[5. 5. 5. 5. 5. 5. 5. 5. 5. 5.]
5. Create an array of all the even integers from 20 to 35
import numpy as np
a=np.arange(20,35,2)
print(a)
[20 22 24 26 28 30 32 34]
6. Create a 3x3 matrix with values ranging from 0 to 8
import numpy as np
a=np.arange(0,9).reshape(3,3)
print(a)
[[0 1 2]
 [3 4 5]
 [6 7 8]]
7. Concatenate a and b
a = np.array([1, 2, 3]), b = np.array([4, 5, 6])
import numpy as np
arr1=np.array([1,2,3])
arr2=np.array([4,5,6])
arr=np.concatenate((arr1,arr2))
print(arr)
[1 2 3 4 5 6]
Pandas
8. Create a dataframe with 3 rows and 2 columns
import pandas as pd
data=[{'a':12,'b':45},{'a':54,'b':23},{'a':94,'b':76}]
df=pd.DataFrame(data)
print(df)
    a   b
0  12  45
1  54  23
2  94  76
9. Generate the series of dates from 1st Jan, 2023 to 10th Feb, 2023
import pandas as pd
a=pd.date_range(start='1/1/2023',end='10/2/2023')
print(a)
DatetimeIndex(['2023-01-01', '2023-01-02', '2023-01-03', '2023-01-04',
               '2023-01-05', '2023-01-06', '2023-01-07', '2023-01-08',
               '2023-01-09', '2023-01-10',
               ...
               '2023-09-23', '2023-09-24', '2023-09-25', '2023-09-26',
               '2023-09-27', '2023-09-28', '2023-09-29', '2023-09-30',
               '2023-10-01', '2023-10-02'],
              dtype='datetime64[ns]', length=275, freq='D')
10. Create 2D list to DataFrame
lists = [[1, 'aaa', 22], [2, 'bbb', 25], [3, 'ccc', 24]]

lists = [[1, 'aaa', 22], [2, 'bbb', 25], [3, 'ccc', 24]]
import pandas as pd
lst=[[1,'aaa',22],[2,'bbb,25'],[3,'ccc',24]]
df=pd.DataFrame(lst)
print(df)
   0       1     2
0  1     aaa  22.0
1  2  bbb,25   NaN
2  3     ccc  24.0
