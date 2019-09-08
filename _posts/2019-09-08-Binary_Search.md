---
layout: post
title: 二分查找
tag: C++,python
---

## C++

c++的二分查找功能需要头文件`<algorithm>`，提供的功能包括查找上界、查找下界、查找是否存在。

`bool binary_search(ForwardIterator first, ForwardIterator last, const T& val)`

* 查找 val 是否在迭代器中

  ```c++
  int a[] = {1,3,5,5,10,13,16};
  binary_search(a, a+6, 5);
  ```

  

`ForwardIterator lower_bound (ForwardIterator first, ForwardIterator last, const T& val)`

* 返回迭代器中第一个大于等于val的值的位置

  ```c++
  int b = lower_bound(a, a+6, 5) - a;	// b = 2
  ```



`ForwardIterator upper_bound (ForwardIterator first, ForwardIterator last, const T& val)`

* 返回迭代器中第一个大于val的值的位置

  ```c++
  int c = upper_bound(a, a+6, 5) - a;	//c = 4
  ```



## Python

python的二分查找存在于`bisect`模块中，提供的功能包括查找上下界，有序插入。

#### 查找

`bisect.bisect_left(a, x, lo=0, hi=len(a))`

* 返回将x有序插入a中位置，若a中有x，则插入在最左边，结果与C++的`lower_bound(a, a+l, x)-a`相同

`bisect.bisect_right(a, x, lo=0, hi=len(a))`

`bisect.bisect(a, x, lo=0, hi=len(a))`

* 返回将x有序插入a中位置，若a中有x，则插入在最右边，结果与C++的`upper_bound(a, a+l, x)-a`相同

#### 插入

`bisect.insort_left(a, x, lo=0, hi=len(a))`

* 将x插入到a中，若a中存在x，则插入在最左边

`bisect.insort_right(a, x, lo=0, hi=len(a))`

`bisect.insort(a, x, lo=0, hi=len(a))`

* 将x插入到a中，若a中存在x，则插入在最右边

