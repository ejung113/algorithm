### 1. 리스트(List)



- 백준 - #11720: 숫자의 합

``` python
n = input()
print(sum(map(int,input())))
```



- 백준 - #2750: 수 정렬하기

``` python
n = int(input())
temp = []
for i in range(n):
  temp.append(int(input()))
temp.sort()
for j in temp:
  print(j)
```



- 정올 - #921: List Comprehension

``` python
n = int(input())
result = [i*i for i in range(1,n+1)]
print(result)
```



- 정올 - #929: List Comprehension

``` python
n = int(input())
result = [f"No.{i}" for i in range(1,n+1)]
print(result)
```



- 백준 - #2562: 최댓값

``` python
a = [int(input()) for i in range(9)]
print(max(a))
print(a.index(max(a))+1)
```



- 정올 - #926: 2차원 리스트

``` python
b = [[list(map(int, input().split())) for _ in range(2)] for i in range(2)]
a1 = b[0]
a2 = b[1]
result = []
for i in range(2):
  for j in range(4):
   a[i][j] = a1[i][j]*a2[i][j]
print(a)
```



- 백준 - #1100: 하얀 칸

``` python
cnt = 0
first = [list(map(str, input())) for _ in range(8)]
for i in range(8):
  for j in range(8):
    if (i+j)%2 == 0:
      if first[i][j] == 'F':
        cnt += 1
print(cnt)
```



### 2. 실습



- 백준 - #2953: 나는 요리사다

``` python
# 1
result = [sum(list(map(int, input().split()))) for i in range(5)]
max_sum_score = max(result)
print(result.index(max_sum_score)+1,max_sum_score)

# 2
temp =[]
for i in range(5):
  score = list(map(int, input().split()))
  sum_score = sum(score)
  temp.append(sum_score)
  max_sum_score = max(temp)
print(temp.index(max_sum_score)+1,max_sum_score)
```

