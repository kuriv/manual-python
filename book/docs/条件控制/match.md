# match

执行下面的代码，进行多路判定。

```python
num = 233
match num:
    case 0:
        print(0)
    case 233:
        print(233)
    case 666:
        print(666)
    case _:
        print('Other')
```

