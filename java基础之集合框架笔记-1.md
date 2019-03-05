###集合框架 API (from CORE JAVA-1)

---

####  java . util . Collection < E >1.2

```
Iterator < E > iterator () 
```

返回一个用于访问集合中每个元素的迭代器 。

​	

```
int size（）
```

 返回当前存储在集合中的元素个数 。 

​	

```
boolean isEmpty（） 
```

如果集合中没有元素 返回 true  。

​	 

```
boolean contains (Object obj)
```

 如果集合中包含了一个与 obj 相等的对象 返回 true  。

​	

```
 boolean containsAll(Collection < ? > other)
```

如果这个集合包含 other 集合中的所有元素, 返回 true。

​	

```
boolean add (Object element)
```

 将一个元素添加到集合中 如果由于这个调用改变了集合 ,返回 true 。

 	

` boolean addAll(Collection <? extends E > other) `

 将 other 集合中的所有元素添加到这个集合 如果由于这个调用改变了集合 ,返回 true 。 

```
boolean remove ( Object obj )
```

 从这个集合中删除等于 obj 的对象 。  如果有匹配的对象被删除 ， 返回 true 。

```
boolean removeAll( Col 1 ection < ? > other ) 
```

从这个集合中删除 other ， 。 集合中存在的所有元素 。 如果由于这个调用改变了集合 返回 true 。

```
default boolean removelf ( Predicate < ? super E > filter ) 
```

JAVA8 从这个集合删除 filter 返回 true 的所有元素 如果由于这个调用改变了集合 则返回 true 。 

```
 void clear ()
```

 从这个集合中删除所有的元素 。

```java
 boolean retainAlll( Collection <? > other )
```

 从这个集合中删除所有与 other 集合中的元素不同的元素 ,如果由于这个调用改变了 集合,  返回 true 。

```java
Object[] toArray ()
```

 返回这个集合的对象数组 。

```java
 < T > T[] toArray ( T[] arrayToFill ) 
```

返回这个集合的对象数组 。

 如果 arrayToFill 足够大, 就将集合中的元素填入这个数组 中 。 剩余空间填补 null ; 否则 ， 分配一个新数组 ， 其成员类型与 arrayToFill 的成员类 型相同， 其长度等于集合的大小,并填充集合元素.

------



####  java . util . Iterator < E >1.2

``` boolean hasNext()```

如果存在可访问的元素 ， 返回 true。



```java
 E next () 
```

返回将要访问的下一个对象 ,如果已经到达了集合的尾部 将拋出一个 NoSuchElementException,返回 true 。



```java
void remove ( )
```

删除上次访问的对象 ,这个方法必须紧跟在访问一个元素之后执行 。如果上次访问后，集合已经发生了变化， 这个方法将抛出一个 IllegalStateException。

