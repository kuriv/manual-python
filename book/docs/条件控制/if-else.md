# if-else

执行下面的代码，进行条件判断。

```python
num = 233
if num > 0:
    print('Yes')
else:
    print('No')
```

条件判断语句可以进行嵌套。

```python
num = 233
if num > 0:
    print('Yes')
    if num > 100:
        print(666)
    else:
        print(num)
else:
    print('No')
```

也可以使用更加简洁的三元表达式。

```python
num = 233
print('Yes') if num > 0 else print('No')
```

