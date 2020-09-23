##### tags : `colde_garage_python_2020`
# 在開始之前你一定要知道的事...
1. python 非常注重縮排
2. python 是一種直譯式語言
3. python 變數的型別不是固定的
4. python 支援大數運算
## 範例
```python=
apple = 1
banana = 0

if apple > banana :
    print("hello")
elif apple == 1:
    print("apple")
else :
    print("world")
    
print(apple)
print(banana)
```
```=
hello
1
0
```
# 如何使用python互動模式
1. Open termial
2. type "python3"
# Hello World
```python=
print("hello world")
```\
# 註解
## 單行註解
```python=
#----單行註解------
```
## 多行註解
```python=
'''
    多
    行
    註
    解
'''
```
# 延序一行文字
'''
sum = 1+\
      2+\
      3
print(sum)
'''
# 字串型態
\\	\	
\'	 '
\"	 "
\n	換行
\r	歸位
\t	Tab
\0	空字元
# python 的資料型態
bool, int, float, complex, str, list, tuple, bytes, bytearray, set, frozenset, dict
# 變數
## 變數型別
* 數值型態：int, float, bool
* 字串型態：str
## 如何使用
```python=
a = 1
b = 1.2
c = True
d = False
e = "hello"
f = 'a'
g = chr(96)
h = 1.5 + 3j
print( type(a) )
print( type(b) )
print( type(c) )
print( type(d) )
print( type(e) )
print( type(f) )
print( type(g) )
print( type(h) )
if type(d) == type(c):
    print(c)
```
```=
<class 'int'>
<class 'float'>
<class 'bool'>
<class 'bool'>
<class 'str'>
<class 'str'>
<class 'str'>
<class 'complex'>
True
```
## 型別轉換
```python=
a = 1
b = float(a)
c = chr(100)
d = ord(c)
print(a, b, c, d)
```
```=
1 1.0 d 100
```
## 關於int
1. 不像 C 的 int 會溢位
2. 非常適合大數運算
# 運算子
* 算術運算子  
+, -, *, /, %, //(取得整除的商數), ** (次方, 7**2 = 49)

* 關係運算子  
==, !=, >, <, >=, <=

* 邏輯運算子  
not, and, or

* 複合指定運算子  
+=, -=, *=, /=, %=, //=, **=
# IO
## input
### python3

```python=
a = input("type what you want to talk: ")
b = input()
c = input()
print(type(a), type(b), type(c))
```
#### input
```
123
23.3
hello
```
#### output
```
<class 'str'> <class 'str'> <class 'str'>
```

```
#### input
```=
123
23.3
"hello"
123
23.3
hello
```
#### output
```=
(<type 'int'>, <type 'float'>, <type 'str'>)
(<type 'str'>, <type 'str'>, <type 'str'>)
```

## print
### useful reference
https://docs.python.org/3/tutorial/inputoutput.html
### most familiar with c printf
```python=
print('%f %d' %( 3.14 , 3))
```
```
3.140000 3
```
### often use print with "format" function
```python
print("{} {}" .format(3.14, 3))
print("{:f} {:d}" .format(3.14, 3))
print("{1:f} {0:d}" .format(3, 3.14))
print("{1:.4f} {0:5d}" .format(3, 3.14))
n1 = 3
n2 = 3.14
print(f'{n1},{n2}')
```
```
3.14 3
3.140000 3
3.140000 3
3.1400     3
3,3.14
```
### print 不換行
```python=
print("hello world " , end="")
print("test")
```
```
hello world test
```

# 條件判斷 (注意本章的所有縮排)
## if, if else, if elif else
```python
a = 1
b = 2
if a < b :
    print("I")
    print("L")
#--------------------
if a > b :
    print("B")
else :
    print("V")
#--------------------  
if a == b :
    print("D")
elif a > b :
    print("E")
else :
    print("P")
    print("Y")
```
```
I
L
V
P
Y
```
## python 沒有 switch case ^ ^
