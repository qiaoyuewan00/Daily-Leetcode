# 处理输入输出

！！！待补充

```python
n, bagweight = map(int, input().split())

weight = list(map(int, input().split()))
value = list(map(int, input().split()))

dp = [[0] * (bagweight + 1) for _ in range(n)]
```

# 字符串

```python
# 查看ASCII码
ord("a")
```



# 列表

```python
del list_1[0] # 移除某个位置的值
list_1.remove(val) # 移除第一个找到等于val的元素
```

## 创建一个矩阵

```python
a列b行的矩阵
matrix =  nums = [[0] * a for _ in range(b)]
```



# 字典

```python
from collections import defaultdict
d = defaultdict(int)  # 初始化加入key的value为0
```



# 类

## Counter：字符串哈希

```
# counter 生成counter, 虽然这里并没有什么用
>>> from collections import Counter
>>> c = Counter('abcasd')
>>> c
Counter({'a': 2, 'c': 1, 'b': 1, 's': 1, 'd': 1})
>>> c2 = Counter(c)
>>> c2
Counter({'a': 2, 'c': 1, 'b': 1, 's': 1, 'd': 1})


>>> c = Counter(['apple', 'pear'])
>>> c['orange']
0

# Counter 间的数学集合操作
>>> c = Counter(a=3, b=1, c=5)
>>> d = Counter(a=1, b=2, d=4)
>>> c + d                       # counter相加, 相同的key的value相加
Counter({'c': 5, 'a': 4, 'd': 4, 'b': 3})
>>> c - d                       # counter相减, 相同的key的value相减，只保留正值得value
```

