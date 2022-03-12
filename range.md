# Range()

`for i in range(1, count):` 是什么意思？

```python
for i in range(1,9):
    print(i)
#输出：1，2，3...8
```

_class_ `range`(_stop_)[¶](https://docs.python.org/zh-cn/3/library/stdtypes.html#range)__

_class_ `range`(_start_, _stop_\[, _step_])

1是start，9是stop，step是默认的1。

`r[i] = start + step*i,i >= 0` 且 `r[i] < stop`。

`r[0] = 1`



用我自己的语言描述：

range()有三种情况

* range(stop)      range:stop->stop-1
* range(start,stop)   range:start->stop-1
* range(start,stop,\[,step] )range:start->stop-1 step&#x20;



``

``

```python
for i in range(0,9):
    print(i)
#输出：0，1，2...8
```

_class_ `range`(_stop_)[¶](https://docs.python.org/zh-cn/3/library/stdtypes.html#range)__

_class_ `range`(_start_, _stop_\[, _step_])

The arguments to the range constructor must be integers (either built-in [`int`](https://docs.python.org/zh-cn/3/library/functions.html#int) or any object that implements the [`__index__()`](https://docs.python.org/zh-cn/3/reference/datamodel.html#object.\_\_index\_\_) special method). If the _step_ argument is omitted, it defaults to `1`. If the _start_ argument is omitted, it defaults to `0`. If _step_ is zero, [`ValueError`](https://docs.python.org/zh-cn/3/library/exceptions.html#ValueError) is raised.

范围构造函数的参数必须是整数（内置 int 或任何实现 **index**() 特殊方法的对象）。如果省略 step 参数，则默认为 1。如果省略 <mark style="color:red;">start</mark> 参数，则默认为 <mark style="color:red;">0</mark>。如果 step 为零，则引发 ValueError。

如果 _step_ 为正值，确定 range `r` 内容的公式为 `r[i] = start + step*i` 其中 `i >= 0` 且 `r[i] < stop`。

如果 _step_ 为负值，确定 range 内容的公式仍然为 `r[i] = start + step*i`，但限制条件改为 `i >= 0` 且 `r[i] > stop`.

如果 `r[0]` 不符合值的限制条件，则该 range 对象为空。 range 对象确实支持负索引，但是会将其解读为从正索引所确定的序列的末尾开始索引。



## range类

{% embed url="https://docs.python.org/zh-cn/3/library/stdtypes.html#typesseq-range" %}

_class_ `range`(_stop_)[¶](https://docs.python.org/zh-cn/3/library/stdtypes.html#range)__

_class_ `range`(_start_, _stop_\[, _step_])

The arguments to the range constructor must be integers (either built-in [`int`](https://docs.python.org/zh-cn/3/library/functions.html#int) or any object that implements the [`__index__()`](https://docs.python.org/zh-cn/3/reference/datamodel.html#object.\_\_index\_\_) special method). If the _step_ argument is omitted, it defaults to `1`. If the _start_ argument is omitted, it defaults to `0`. If _step_ is zero, [`ValueError`](https://docs.python.org/zh-cn/3/library/exceptions.html#ValueError) is raised.

范围构造函数的参数必须是整数（内置 int 或任何实现 **index**() 特殊方法的对象）。如果省略 step 参数，则默认为 1。如果省略 <mark style="color:red;">start</mark> 参数，则默认为 <mark style="color:red;">0</mark>。如果 step 为零，则引发 ValueError。

如果 _step_ 为正值，确定 range `r` 内容的公式为 `r[i] = start + step*i` 其中 `i >= 0` 且 `r[i] < stop`。

如果 _step_ 为负值，确定 range 内容的公式仍然为 `r[i] = start + step*i`，但限制条件改为 `i >= 0` 且 `r[i] > stop`.

如果 `r[0]` 不符合值的限制条件，则该 range 对象为空。 range 对象确实支持负索引，但是会将其解读为从正索引所确定的序列的末尾开始索引。

## for循环

{% embed url="https://docs.python.org/zh-cn/3/tutorial/controlflow.html#for-statements" %}

## range()函数

{% embed url="https://docs.python.org/zh-cn/3/tutorial/controlflow.html#the-range-function" %}
