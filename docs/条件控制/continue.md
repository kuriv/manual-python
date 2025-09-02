# continue

执行下面的代码，在循环中根据指定条件进行下一次循环。

```python
num = 9
while num > 0:
    if num == 6:
        num -= 1
        continue
    print(num)
    num -= 1
```

