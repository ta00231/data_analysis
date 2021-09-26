# Python基础补充（2）

## 1、Tab补全可查看对象拥有的属性和方法


```python
a = 'foo'
```

## 2、getattr(x, 'y') 等价于x.y


```python
getattr(a,'split')
```




    <function str.split(sep=None, maxsplit=-1)>




```python
a.split
```




    <function str.split(sep=None, maxsplit=-1)>



## 3、datetime模块


```python
from datetime import datetime, date, time
```


```python
dt = datetime(2021, 9, 25, 9, 57, 40)
```


```python
dt.day
```




    25




```python
dt.month
```




    9




```python
dt.hour
```




    9



### 格式化字符串


```python
dt.strftime('%m/%d/%y %H:%M:%S')
```




    '09/25/21 09:57:40'




```python
datetime.strptime('20210925', '%Y%m%d')
```




    datetime.datetime(2021, 9, 25, 0, 0)



![5.png](https://github.com/ta00231/data_analysis/blob/main/picture/5.png)
格式化对应表格

## 4、⼆分搜索和维护已排序的列表

### bisect模块


```python
import bisect as bt
```


```python
c = [1,2,2,2,3,4,7]
```

#### bisect.bisect可以找到插⼊值后仍保证排序的位置


```python
bt.bisect(c, 2)
```




    4




```python
bt.bisect(c, 5)
```




    6



#### bisect.insort是找出的位置插⼊值


```python
bt.insort(c, 6)
```


```python
c
```




    [1, 2, 2, 2, 3, 4, 6, 7]



#### bisect模块不会检查列表是否已排好序，进⾏检查的话会耗费⼤量计算。因此，对未排序的列表使⽤bisect不会产⽣错误，但结果不⼀定正确。
