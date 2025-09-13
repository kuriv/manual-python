# os

执行下面的代码，获取操作系统类型。

```python
import os

print(os.name)
```

执行下面的代码，获取系统环境变量。

```python
import os

print(os.getenv('path'))
```

执行下面的代码，获取当前路径的绝对路径。

```python
import os

print(os.path.abspath('.'))
```

执行下面的代码，获取指定路径的文件名。

```python
import os

print(os.path.basename(__file__))
```

执行下面的代码，获取指定路径的目录名。

```python
import os

print(os.path.dirname(__file__))
```

执行下面的代码，判断指定文件是否存在。

```python
import os

print(os.path.isfile(__file__))
```

执行下面的代码，判断指定目录是否存在。

```python
import os

print(os.path.isdir(os.path.dirname(__file__)))
```

