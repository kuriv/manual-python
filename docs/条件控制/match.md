# match

执行下面的代码，进行多路判定。

```python
num = 233
match num:
    case 0:
        print('foo')
    case 233:
        print('bar')
    case 666:
        print('baz')
    case _:
        print('qux')
```

