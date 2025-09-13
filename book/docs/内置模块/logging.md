# logging

执行下面的代码，记录日志。

```python
import logging

logging.debug('debug message')
logging.info('info message')
logging.warning('warning message')
logging.error('error message')
logging.critical('critical message')
```

执行下面的代码，指定日志文件的文件名。

```python
import logging

logging.basicConfig(filename='demo.log')
logging.debug('debug message')
logging.info('info message')
logging.warning('warning message')
logging.error('error message')
logging.critical('critical message')
```

执行下面的代码，指定日志文件的文件名和显示级别。

```python
import logging

logging.basicConfig(filename='demo.log', filemode='a', level=logging.DEBUG)
logging.debug('debug message')
logging.info('info message')
logging.warning('warning message')
logging.error('error message')
logging.critical('critical message')
```

执行下面的代码，指定日志文件的输出格式。

```python
import logging

logging.basicConfig(filename='demo.log', filemode='w', level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')
logging.debug('debug message')
logging.info('info message')
logging.warning('warning message')
logging.error('error message')
logging.critical('critical message')
```

