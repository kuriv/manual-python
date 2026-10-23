# for

执行下面的代码，进行条件循环。

```python
for i in range(1, 10):
    print(i)
```

条件循环末尾可搭配条件判断语句。

```python
for i in range(1, 10):
    print(i)
else:
    print('End')
```

条件循环也可以嵌套。

```python
matrix = []
for i in range(3):
    row = []
    for j in range(3):
        row.append(0)
    matrix.append(row)
print(matrix)
```

还可以使用推导式来生成多维矩阵。

```python
matrix = [[0 for j in range(3)] for i in range(3)]
print(matrix)
```

