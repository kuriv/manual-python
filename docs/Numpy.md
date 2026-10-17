# Numpy

执行下面的命令，安装 Numpy 扩展模块。

```
pip install numpy
```

执行下面的代码，验证是否安装成功。

```python
import numpy as np

print(np.__version__)
```

执行下面的代码，获取指定数组的维度。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.ndim)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.ndim)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.ndim)
```

执行下面的代码，获取指定数组的形状，并以行数与列数的方式返回。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.shape)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.shape)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.shape)
```

执行下面的代码，获取指定数组中元素的总数。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.size)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.size)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.size)
```

执行下面的代码，获取指定数组中元素的数据类型。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.dtype)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.dtype)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.dtype)
```

执行下面的代码，转置指定的数组，即将数组的行列互换，只对二维数组才有效果。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr)
print(arr.T)
```

执行下面的代码，获取指定数组中单个元素占用内存的字节数。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.itemsize)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.itemsize)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.itemsize)
```

执行下面的代码，获取指定数组占用内存总字节数。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.nbytes, arr.size * arr.itemsize)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.nbytes, arr.size * arr.itemsize)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.nbytes, arr.size * arr.itemsize)
```

执行下面的代码，获取指定数组的内存标记信息。

```python
import numpy as np

arr = np.array(2.33)
print(arr, arr.flags)
arr = np.array(['foo', 'bar', 'baz'])
print(arr, arr.flags)
arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr, arr.flags)
```

也可以通过下面的方式来创建指定的数组。

```python
import numpy as np

arr = np.array([1, 2, 3], dtype=np.float64)
print(arr, arr.dtype)
```

执行下面的代码，深拷贝并创建指定的新数组，修改新数组不会影响原数组。

```python
import numpy as np

arr1 = np.array([1, 2, 3])
arr2 = np.copy(arr1)
arr2[0] = 2
print(arr1)
print(arr2)
```

执行下面的代码，创建全部元素为 0 的数组。

```python
import numpy as np

arr = np.zeros((2, 3))
print(arr, arr.dtype)
arr = np.zeros((2, 3), dtype=np.int64)
print(arr, arr.dtype)
```

执行下面的代码，创建全部元素为 1 的数组。

```python
import numpy as np

arr = np.ones((2, 3))
print(arr, arr.dtype)
arr = np.ones((2, 3), dtype=np.int64)
print(arr, arr.dtype)
```

执行下面的代码，创建指定形状的数组，但不初始化值，内存残留垃圾值。

```python
import numpy as np

arr = np.empty((2, 3))
print(arr)
```

执行下面的代码，创建指定形状的数组，所有元素统一填充指定值。

```python
import numpy as np

arr = np.full((2, 3), 1.23)
print(arr)
```

执行下面的代码，生成与原数组形状和数据类型完全相同的新数组，其中所有元素全部为 0 。

```python
import numpy as np

arr = np.array([1, 2, 3], dtype=np.float64)
print(arr)
arr = np.zeros_like(arr)
print(arr)
```

执行下面的代码，生成与原数组形状和数据类型完全相同的新数组，其中所有元素全部为 1 。

```python
import numpy as np

arr = np.array([1, 2, 3], dtype=np.float64)
print(arr)
arr = np.ones_like(arr)
print(arr)
```

执行下面的代码，生成与原数组形状和数据类型完全相同的新数组，但不初始化值。

```python
import numpy as np

arr = np.array([1, 2, 3], dtype=np.float64)
print(arr)
arr = np.empty_like(arr)
print(arr)
```

执行下面的代码，生成与原数组形状和数据类型完全相同的新数组，并统一填充指定值。

```python
import numpy as np

arr = np.array([1, 2, 3], dtype=np.float64)
print(arr)
arr = np.full_like(arr, 1.23)
print(arr)
```

执行下面的代码，生成指定的等差序列数组。

```python
import numpy as np

arr = np.arange(1, 10, 2)
print(arr)
```

执行下面的代码，在指定数字区间，均匀生成若干个间距等分的数组。

```python
import numpy as np

arr = np.linspace(0, 1, 5)
print(arr)
arr = np.linspace(0, 100, 5, dtype=np.int64)
print(arr)
```

执行下面的代码，在指定指数区间，均匀生成若干个对数等分的数组。

```python
import numpy as np

arr = np.logspace(0, 2, 3)
print(arr)
arr = np.logspace(1, 4, 4, base=2)
print(arr)
```

执行下面的代码，生成指定的单位矩阵数组，主对角线位置元素全为 1 ，其余位置元素全为 0 。

```python
import numpy as np

arr = np.eye(3)
print(arr)
```

执行下面的代码，生成指定的对角矩阵数组，也可以用来提取对角线元素。

```python
import numpy as np

arr = np.diag([1, 2, 3])
print(arr)
arr = np.diag([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr)
```

执行下面的代码，创建指定形状的数组，均匀生成并填充 0 ~ 1 区间的随机浮点数。

```python
import numpy as np

arr = np.random.rand(2, 3)
print(arr)
```

执行下面的代码，创建指定形状的数组，均匀生成并填充指定数字区间的随机浮点数。

```python
import numpy as np

arr = np.random.uniform(2, 5, (2, 3))
print(arr)
```

执行下面的代码，创建指定形状的数组，均匀生成并填充指定数字区间的随机整数。

```python
import numpy as np

arr = np.random.randint(2, 5, (2, 3))
print(arr)
```

执行下面的代码，创建指定形状的数组，并生成标准正态分布的随机浮点数。

```python
import numpy as np

arr = np.random.randn(2, 3)
print(arr)
```

执行下面的代码，设置随机种子，用来固定随机数。

```python
import numpy as np

np.random.seed(666)
print(np.random.rand(2, 3))
np.random.seed(666)
print(np.random.rand(2, 3))
```

在 Numpy 中，数组同样支持索引、截取。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr)
print(arr[0])
print(arr[-1])
print(arr[:])
print(arr[1:2])
print(arr[2:])
print(arr[-1:])
print(arr[:-1])
print(arr[-1::-1])
print(arr[2][2], arr[2, 2])
print(arr[:, 1])
print(arr[1, :])
print(arr[0:2, :])
print(arr[:, 0:2])
print(arr > 4)
print(arr[arr > 4])
```

执行下面的代码，对指定的数组进行算数运算。

```python
import numpy as np

arr1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
arr2 = np.array([[9, 8, 7], [6, 5, 4], [3, 2, 1]])
print(arr1 + arr2)
print(arr1 - arr2)
print(arr1 * arr2)
print(arr1 / arr2)
print(arr1 // arr2)
```

两个形状不同的数组，只要满足广播机制也可以进行算数运算。

```python
import numpy as np

arr1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
arr2 = np.array([[1], [2], [3]])
print(arr1 + 1)
print(arr1 - 1)
print(arr1 * 2)
print(arr1 / 2)
print(arr1 % 2)
print(arr1 ** 2)
print(arr1 + arr2)
print(arr1 - arr2)
print(arr1 * arr2)
print(arr1 / arr2)
print(arr1 // arr2)
```

执行下面的代码，对指定的数据进行线性代数矩阵相乘运算。

```python
import numpy as np

arr1 = np.array([[1, 2, 3], [4, 5, 6]])
arr2 = np.array([[1], [2], [3]])
print(arr1 @ arr2)
```

执行下面的代码，对指定数组中每一个元素计算平方根。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.sqrt(arr))
print(arr ** 0.5)
```

执行下面的代码，对指定数组中每一个元素计算幂值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.pow(arr, 2))
print(arr ** 2)
```

执行下面的代码，对指定数组中每一个元素计算绝对值。

```python
import numpy as np

arr = np.array([[-1, 2, 3], [4, -5, 6], [7, 8, -9]])
print(np.abs(arr))
```

执行下面的代码，对指定数组中每一个元素进行四舍五入。

```python
import numpy as np

arr = np.array([1.2, 1.5, 1.7, -2.3, -2.6])
print(np.round(arr))
```

执行下面的代码，对指定数组中每一个元素进行向上取整。

```python
import numpy as np

arr = np.array([1.2, 1.5, 1.7, -2.3, -2.6])
print(np.ceil(arr))
```

执行下面的代码，对指定数组中每一个元素进行向下取整。

```python
import numpy as np

arr = np.array([1.2, 1.5, 1.7, -2.3, -2.6])
print(np.floor(arr))
```

执行下面的代码，计算指定数组中所有元素的总和。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.sum(arr))
```

执行下面的代码，对指定数组中所有元素进行累积求和运算，会保留每一步中间结果。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.cumsum(arr))
```

执行下面的代码，计算指定数组中所有元素的乘积。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.prod(arr))
```

执行下面的代码，对指定数组中所有元素进行累积乘积运算，会保留每一步中间结果。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.cumprod(arr))
```

执行下面的代码，计算指定数组中所有元素的平均值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.mean(arr))
```

执行下面的代码，计算指定数组中所有元素的最大值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.max(arr))
```

执行下面的代码，获取指定数组中元素最大值的下标。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.argmax(arr))
print(np.argmax(arr, axis=0))
print(np.argmax(arr, axis=1))
```

执行下面的代码，计算指定数组中所有元素的最小值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.min(arr))
```

执行下面的代码，获取指定数组中元素最小值的下标。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.argmin(arr))
print(np.argmin(arr, axis=0))
print(np.argmin(arr, axis=1))
```

执行下面的代码，计算指定数组中的中位数，中位数不受极端大数小数的影响。

```python
import numpy as np

arr = np.array([[-100, -99, -98], [1, 2, 3], [98, 99, 100]])
print(np.median(arr))
arr = np.array([[-100, -99], [1, 2], [99, 100]])
print(np.median(arr))
```

执行下面的代码，计算指定数组的方差，主要用于衡量数据离散程度，数据波动越大方差越大。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.var(arr))
arr = np.array([[-10000, -1000, -100], [1, 3, 5], [100, 1000, 10000]])
print(np.var(arr))
```

执行下面的代码，计算指定数组的标准差，等同于方差的平方根。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.std(arr))
arr = np.array([[-10000, -1000, -100], [1, 3, 5], [100, 1000, 10000]])
print(np.std(arr))
```

执行下面的代码，计算指定数组的百分位数。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.percentile(arr, 0))
print(np.percentile(arr, 50))
print(np.percentile(arr, 100))
print(np.percentile(arr, 50, axis=0))
print(np.percentile(arr, 50, axis=1))
```

执行下面的代码，对指定数组中每一个元素计算自然指数。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.exp(arr))
```

执行下面的代码，对指定数组中每一个元素计算自然对数。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.log(arr))
```

执行下面的代码，对指定数组中每一个元素计算正弦值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.sin(arr))
```

执行下面的代码，对指定数组中每一个元素计算余弦值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.cos(arr))
```

执行下面的代码，对指定数组中每一个元素计算正切值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.tan(arr))
```

执行下面的代码，比较指定的两个数组中所有元素是否相等。

```python
import numpy as np

arr1 = np.array([1, 3, 5])
arr2 = np.array([6, 4, 2])
print(np.equal(arr1, arr2))
print(arr1 == arr2)
```

执行下面的代码，比较指定的两个数组中所有元素是否不相等。

```python
import numpy as np

arr1 = np.array([1, 3, 5])
arr2 = np.array([6, 4, 2])
print(np.not_equal(arr1, arr2))
print(arr1 != arr2)
```

执行下面的代码，判断指定数组中所有元素是否大于另一个数组。

```python
import numpy as np

arr1 = np.array([1, 3, 5])
arr2 = np.array([6, 4, 2])
print(np.greater(arr1, arr2))
print(arr1 > arr2)
```

执行下面的代码，判断指定数组中所有元素是大于等于另一个数组。

```python
import numpy as np

arr1 = np.array([1, 3, 5])
arr2 = np.array([6, 4, 2])
print(np.greater_equal(arr1, arr2))
print(arr1 >= arr2)
```

执行下面的代码，判断指定数组中所有元素是否小于另一个数组。

```python
import numpy as np

arr1 = np.array([1, 3, 5])
arr2 = np.array([6, 4, 2])
print(np.less(arr1, arr2))
print(arr1 < arr2)
```

执行下面的代码，判断指定数组中所有元素是否小于等于另一个数组。

```python
import numpy as np

arr1 = np.array([1, 3, 5])
arr2 = np.array([6, 4, 2])
print(np.less_equal(arr1, arr2))
print(arr1 <= arr2)
```

执行下面的代码，组合多个筛选条件并进行逻辑与运算。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.logical_and(arr > 3, arr < 7))
print(arr[np.logical_and(arr > 3, arr < 7)])
print((arr > 3) & (arr < 7))
print(arr[(arr > 3) & (arr < 7)])
```

执行下面的代码，组合多个筛选条件并进行逻辑或运算。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.logical_or(arr < 3, arr > 7))
print(arr[np.logical_or(arr < 3, arr > 7)])
print((arr < 3) | (arr > 7))
print(arr[(arr < 3) | (arr > 7)])
```

执行下面的代码，组合指定的筛选条件并进行逻辑非运算。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.logical_not(arr > 5))
print(arr[np.logical_not(arr > 5)])
print(~(arr > 5))
print(arr[~(arr > 5)])
```

执行下面的代码，聚合筛选条件并返回结果，只要存在一个结果为真则返回真。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.any(arr > 5))
```

执行下面的代码，聚合筛选条件并返回结果，只有所有结果全部为真则返回真。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.all(arr > 5))
```

执行下面的代码，查找满足条件的元素下标并返回行列索引数组，也可以用来进行条件查找后赋值。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(np.where(arr > 5))
print(np.where(arr > 5, True, False))
print(np.where(arr > 5, arr, -1))
```

执行下面的代码，对指定的数组进行多条件分支选择。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
condlist = [(arr < 5), (arr >= 5) & (arr < 7), (arr >= 7)]
choicelist = [1, 0, -1]
print(np.select(condlist=condlist, choicelist=choicelist))
```

执行下面的代码，对指定的数组进行排序。

```python
import numpy as np

arr = np.array([[3, 1, 2], [6, 4, 5], [9, 7, 8]])
print(np.sort(arr))
print(np.sort(arr, axis=0))
print(np.sort(arr, axis=1))
```

执行下面的代码，返回指定数组排序后元素对应的下标索引。

```python
import numpy as np

arr = np.array([[3, 1, 2], [6, 4, 5], [9, 7, 8]])
print(np.argsort(arr))
print(np.argsort(arr, axis=0))
print(np.argsort(arr, axis=1))
```

执行下面的代码，将指定的数组去重，并返回排序后的结果。

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 2, 6], [7, 2, 9]])
print(np.unique(arr))
```

执行下面的代码，拼接指定的多个数组。

```python
import numpy as np

arr1 = np.array([[1, 2, 3], [4, 5, 6]])
arr2 = np.array([[6, 5, 4], [3, 2, 1]])
print(np.concatenate([arr1, arr2]))
print(np.concatenate([arr1, arr2], axis=0))
print(np.concatenate([arr1, arr2], axis=1))
```

执行下面的代码，将指定的数组分割成多个数组。

```python
import numpy as np

arr = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])
print(np.split(arr, 2))
print(np.split(arr, 2, axis=0))
print(np.split(arr, 4, axis=1))
```

执行下面的代码，重新修改指定数组的形状。

```python
import numpy as np

arr = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
print(arr)
print(np.reshape(arr, (2, 4)))
print(np.reshape(arr, (1, 8)))
print(np.reshape(arr, (-1, 4)))
print(np.reshape(arr, (1, -1)))
```

