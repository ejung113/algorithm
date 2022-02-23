### 1. 기본 입출력



- 백준 - #1000: A+B

``` python
a ,b = map(int, input().split())
print(a+b)
```



- 백준 - #2558: A+B-2

``` python
a = int(input())
b = int(input())
print(a+b)
```



- 백준 - #10950: A+B-3

``` python
T = int(input())
for i in range(T):
  a, b = map(int, input().split())
  print(a+b)
```



- 백준 - #10953: A+B-6

``` python
T = int(input())
for i in range(T):
  a, b = map(int, input().split(","))
  print(a+b)
```



- 백준 - #11021: A+B-7

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



- 백준 - #11022: A+B-8

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



- 백준 - #2438: 별 찍기 - 1

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



- 백준 - #2439: 별 찍기 - 2

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



### 2. 문자열(String)



- 백준 - #10988: 팰린드롬인지 확인하기

``` python
word = input()
if list(word) == list(word)[::-1]:
  print("1")
else:
  print("0")
```



- 백준 - #2711: 오타맨 고창영

``` python
# 1
num = int(input())
for i in range(num):
  S = input()
  R = S.split(" ")
  T = int(R[0])
  word = R[1]
  print(word[:T-1]+word[T:])

# 2
t = int(input())
for i in range(t):    
	index, word = input().split()    
	index = int(index)    
	changed_word = word[:index-1] + word[index:]    
	print(changed_word)
```



- 백준 - #17249: 태보태보 총난타

``` python
T = str(input())
S = T.split("(^0^)")
print(S[0].count("@"),S[1].count("@"))
```



- 백준 - #2789: 유학 금지

``` python
word = list(input())
cam = list("CAMBRIDGE")
for i in range(len(word)):
  if word[i] not in cam:
    print(word[i],end="")
```

