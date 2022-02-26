### 1. 딕셔너리(Dictionary)



- 정올 - #945: 기타 자료형

``` python
a = {"Pokemon":"Pikachu", "Digimon":"Agumon", "Yugioh":"Black Magician"}
b = input()
if b not in a:
  print("I don't know")
else:
  print(a.get(b))
```



- 정올 - #946: 기타 자료형

``` python
# 1
temp = []
num = int(input())
for i in range(num):
  con_cap = list(map(str, input().split()))
  temp.append(con_cap)
dict = {temp[i][0]:temp[i][1] for i in range(num)}

country = input()
if country not in dict:
  print("I don't know")
else:
  print(dict.get(country))

# 2
num = int(input())
dict = {}
for i in range(num):
  country, capital = input().split()
  dict[country] = capital
country_1 = input()
print(dic.get(country_1, "I don't know"))
```



- 정올 - #953: 기타 자료형

``` python
dic = {}
names = list(map(str, input().split()))
for name in names:
    if name not in dic:
        dic[name] = 1 
    else:
        dic[name] += 1
for key in dic.keys():
    if dic[key] == min(dic.values()):
        print(key)
print(min(dic.values()))
```



### 2. 카카오 기출



```python
def solution(s):
    nums = {"zero": "0", "one": "1", "two": "2", "three": "3", "four": "4", "five": "5", "six": "6", "seven": "7", "eight": "8", "nine": "9"}
    for key in num:
        if num_list[i] in s:
            s = s.replace(num_list[i],nums[num_list[i]])
    return int(s)
```



