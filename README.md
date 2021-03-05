# python_class

- 3/5









```
movie_rank = ["닥터 스트레인지","스플릿","럭키"]
movie_rank.append("배트맨")
print(movie_rank)
movie_rank.insert(1,"슈퍼맨")
print(movie_rank)
del movie_rank[3:4]
print(movie_rank)
del movie_rank[2:5]
print(movie_rank)
```

- 3/3

```
temp = reversed([1,2,3,4,5,6])
numbers = [1,2,3,4,5,6]

for i in reversed(numbers):
  print("첫번쨰 반복문 : {}".format(i))

for i in reversed(numbers):
  print("두번쨰 반복문 : {}".format(i))
 ```
 ```def search_list(a, x):
  for i in range(len(a)):
    if x == a[i]:
      return i
  return -1

v = [17,92,18,33,58,7,33,42]
print(search_list(v,18))
```
```def find_min_idx(a):
  n = len(a)
  min_idx = 0
  for i in range(1,n):
    if a[i] < a[min_idx]:
      min_idx = i
    return min_idx

def sel_sort(a):
  result = []
  while a:
    min_idx = find_min_idx(a)
    value = a.pop(min_idx)
    result.append(value)
  return result
d = [2,4,5,1,3]
print(sel_sort(d))
```
```
def sel_sort(a):
  n=len(a)
  for i in range(0, n-1):
    min_idx = i
    for j in range(i+1, n):
      if a[j] < a[min_idx]:
        min_idx = j
        a[i], a[min_idx] = a[min_idx], a[i]

d = [2,4,5,1,3]
sel_sort(d)
print(d)
```

- 2/26

- 집합

- add(x) : 집합에 자료 x를 추가
- discard(x) : 집합에 자료 x가 들어 있다면 삭제
- clear() : 집합에 모든 자료를 지움

- x in s : 어떤 자료 x가 집합 s에 들어있는지 확인
- x not in s : 반대

- 2/24

- len(a) : 리스트 길이(자료 개수)를 구함
- append(x) : 자료 x를 리스트의 맨 뒤에 추가
- insert(i,x) : 리스트의 i번 위치에 x를 추가
- pop(i) : i번 위치에 있는 자료를 리스트에서 제거 단, 지정하지 않으면 마지막값으로 추출 
- clear() : 리스트의 모든 자료를 지움, 포기화
- x in a : 어떤 자료 x가 리스트 a 안에 있는지 확인 반대결과 (x not in a)

- 집합 순서 상관 X

- 2/22

- isalnum() : 문자열이 알파벳 또는 숫자로만 구성되어있는지 확인
- isalpha() : 문자열이 알파벳으로만 구성되어있는지 확인
- isdecimal() : 문자열이 정수 형태인지 확인
- isdigit() : 문자열이 숫자로 인식 될 수 있는 것인지 확인
- islower() : 문자열이 소문자로만 구성되어 있는지 확인
- isupper() : 문자열이 대문자로만 구성되어 있는지 확인

```
-list_a = [1,2,3,4,5,6,7,8,9,10]
-list_a.remove(10)
-print(list_a)
-[1,2,3,4,5,6,7,8,9]
-list_a.clear()
-print(list_a)
-[]
```
```
-list_a = [1,2,3,4,5,6,7,8,9,10]
-10 in list_a
-ture
-11 in list_a
false
-10 not in list_a
-false
-11 not in list_a
-ture
```
