`data.shape` 表示维度大小
`data.dtype` 表示`data type`
```
In [1]: data1 = [6,7.5,8,0,1]

In [2]: import numpy as np 

In [3]: arr1 = np.array(data1)

In [4]: arr1
Out[4]: array([6. , 7.5, 8. , 0. , 1. ])

```
np 的数组进行是点对点操作 
可以不在使用for循环的情况下
计算出俩个相同维度数组的+-*/

```
In [59]: arr2 = np.array([[0.,0.,1.],[7.,2.,12.]])

In [60]: arr2
Out[60]: 
array([[ 0.,  0.,  1.],
       [ 7.,  2., 12.]])

In [61]: arr2 > arr
Out[61]: 
array([[False, False, False],
       [ True, False,  True]])
```
生成布尔数组


```
In [68]: arr
Out[68]: array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])

In [69]: arr[5:8] = 12

In [70]: arr
Out[70]: array([ 0,  1,  2,  3,  4, 12, 12, 12,  8,  9])
```
产生了广式转变  array切片的结果只是一个view
用来代表原来array对应的元素