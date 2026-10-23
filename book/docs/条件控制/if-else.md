# if-else

执行下面的代码，进行条件判断。

```python
num = 233
if num > 0:
    print(True)
else:
    print(False)
```

条件判断语句可以嵌套。

```python
num = 233
if num > 0:
    print(True)
    if num > 100:
        print('Hello Python!')
    else:
        print('Hello World!')
else:
    print(False)
```

也可以使用更加简洁的三元表达式。

```python
num = 233
print(True) if num > 0 else print(False)
```

