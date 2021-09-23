# 测试


```python
print('hello world')
```

    hello world
    

# Python基础补充

## 1、内省

### ?:显示变量信息或者函数信息，一般为''' ''' 包含的文档注释内容

### ??:显示函数源代码

如下为相关操作演示：


```python
b = [1,2.3]
```


```python
b?
```

![image.png](attachment:image.png)


```python
print?
```

![image.png](attachment:image.png)


```python
def Sum(a, b):
    '''
    function : get the result of a plus b
    parameters : a , b
    return : sum
    '''
    sum = a + b
    return sum
```


```python
Sum?
```

![image.png](attachment:image.png)


```python
Sum??
```

![image.png](attachment:image.png)
