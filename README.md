# python_class

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
