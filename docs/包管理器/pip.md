# pip

pip 是 Python 的包管理工具。打开命令行，执行下面的命令，列出已安装的 Python 包及其版本号。

```
pip list
```

执行下面的命令，安装指定的 Python 包。

```
pip install numpy
```

执行下面的命令，卸载指定的 Python 包。

```
pip uninstall numpy
```

执行下面的代码，验证是否安装成功。

```python
import numpy

print(numpy.__version__)
```

