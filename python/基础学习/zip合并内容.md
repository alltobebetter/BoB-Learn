# Zip 可迭代内容合并

`zip` 是 Python 的一个内置函数，它用于将多个可迭代对象（例如列表、元组、字符串等）打包成一个迭代器，返回一个元组的迭代器。每个元组包含来自输入可迭代对象的对应元素。

**基本用法**

```python
list1 = [1, 2, 3]
list2 = ['a', 'b', 'c']

zipped = zip(list1, list2)

print(zipped)  # 输出：<zip object at 0x...>  注意：zip 返回的是一个迭代器对象

for item in zipped:
    print(item) # 输出：(1, 'a') (2, 'b') (3, 'c')

# 将 zip 对象转换为列表
zipped_list = list(zip(list1, list2))
print(zipped_list)  # 输出：[(1, 'a'), (2, 'b'), (3, 'c')]


# 可以打包多个可迭代对象
list3 = [True, False, True]
zipped_multiple = list(zip(list1, list2, list3))
print(zipped_multiple) # 输出：[(1, 'a', True), (2, 'b', False), (3, 'c', True)]
```

**长度不一致**

当输入的可迭代对象长度不一致时，`zip` 会以最短的序列为准，忽略多余的元素。

```python
list1 = [1, 2, 3, 4]
list2 = ['a', 'b', 'c']

zipped = list(zip(list1, list2))
print(zipped)  # 输出：[(1, 'a'), (2, 'b'), (3, 'c')]  # 4 被忽略了
```

**`zip_longest`**

如果希望处理长度不一致的情况，并用填充值填充缺失的元素，可以使用 `itertools` 模块中的 `zip_longest` 函数。

```python
from itertools import zip_longest

list1 = [1, 2, 3]
list2 = ['a', 'b', 'c', 'd']

zipped = list(zip_longest(list1, list2, fillvalue='-'))  # 使用 '-' 填充缺失值, 默认是 None.
print(zipped)  # 输出：[(1, 'a'), (2, 'b'), (3, 'c'), ('-', 'd')]
```

**解压**

可以使用 `zip(*)` 来解压一个已打包的序列。

```python
zipped = [(1, 'a'), (2, 'b'), (3, 'c')]
unzipped = list(zip(*zipped))
print(unzipped)  # 输出：[(1, 2, 3), ('a', 'b', 'c')]
```


**常用场景**

* **并行迭代:**  同时遍历多个序列。
* **创建字典:**  将两个列表打包成键值对，然后转换成字典。

   ```python
   keys = ['name', 'age', 'city']
   values = ['Alice', 30, 'New York']
   my_dict = dict(zip(keys, values))
   print(my_dict)  # 输出：{'name': 'Alice', 'age': 30, 'city': 'New York'}
   ```

* **数据处理和转换:** 在数据处理中，`zip` 经常用于将数据按列重新组合或进行其他操作。
实用且灵活的函数，可以方便地处理多个序列的并行迭代和数据转换等任务。  理解它的工作原理和用法，可以 significantly 提高你的 Python 编程效率.
