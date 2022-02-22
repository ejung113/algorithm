### 기본 입출력

#### 백준 - #1000: A+B

``` python
a ,b = map(int, input().split())
print(a+b)
```



#### 백준 - #2558: A+B-2

``` python
a = int(input())
b = int(input())
print(a+b)
```



#### 백준 - #10950: A+B-3

``` python
T = int(input())
for i in range(T):
  a, b = map(int, input().split())
  print(a+b)
```



#### 백준 - #10953: A+B-6

``` python
T = int(input())
for i in range(T):
  a, b = map(int, input().split(","))
  print(a+b)
```



#### 백준 - #11021: A+B-7

``` python
# 1
T = int(input())
for i in range(T):
  a, b = map(int, input().split())
  print(f"Case #{i+1}:",a+b)

# 2
T = int(input())
for i in range(T):
  a, b = map(int, input().split())
  print(f"Case #{i+1}: {a+b}")
```



#### 백준 - #11022: A+B-8

``` python
# 1
T = int(input())
for i in range(T):
  a, b = map(int, input().split())
  print(f"Case #{i+1}:",a,"+",b,"=",a+b)

# 2
T = int(input())
for i in range(T):
  a, b = map(int, input().split())
  print(f"Case #{i+1}: {a} + {b} = {a+b}")
```



#### 백준 - #2438: 별 찍기 - 1

``` python
# 1
T = int(input())
for i in range(1, T+1):
  for j in range(i):
    print("*",end="")
  print()

# 2
T = int(input())
for i in range(1, T+1):
	print("*"*i)
```



#### 백준 - #2439: 별 찍기 - 2

``` python
# 1
N = int(input())
for i in range(1, N+1):
  for j in range(N-i):
    print(" ",end="")
  for j in range(i):
    print("*",end="")
  print()

# 2
T = int(input())
for i in range(1, T+1):
	print(" "*(N-i)+"*"*i)
```