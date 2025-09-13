# time

执行下面的代码，推迟程序执行。

```python
import time

print('Hello World!')
time.sleep(2)
print('Hello Python!')
```

执行下面的代码，获取当前时间戳。

```python
import time

print(time.time())
```

执行下面的代码，格式化时间戳为本地时间。

```python
import time

print(time.localtime())
```

执行下面的代码，获取系统当前时间。

```python
import time

print(time.asctime())
```

执行下面的代码，将时间戳转换为系统时间格式。

```python
import time

print(time.ctime(time.time()))
```

执行下面的代码，返回字符串格式化的时间。

```python
import time

print(time.strftime('%Y-%m-%d %H:%M:%S', time.localtime()))
```
