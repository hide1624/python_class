# python_class

ArrayList 클래스의 주요 매서드

boolean add(E e) : 요소 하나를 배열에 추가합니다. E는 요소의 자료형을 의미합니다.
int size() : 배열에 추가된 요소 전체 개수를 변환합니다.
E get(int index) : 배열에 index 위치에 있는 요소 값을 변환합니다.
E remove(int index) : 배열에 index 위치에 있는 요소 값을 제거하고 그 값을 반환합니다.
boolean isEmpty() : 배열에 비어 있는지 확인합니다.

- 5/14

- 파이선 while for 문 1부터 50까지의 
		int num = 1;
		int sum = 0;
		
		while(num <= 50) {
			sum += num;
			num++;
		}
		System.out.println("1부터 50까지의 합은" + sum + "입니다.");
		
		int i;
		int hap;
		for(i = 1, hap = 0; i <= 50; i++) {
			hap += i;
		}
		System.out.println("1부터 50까지의 합은" + hap + "입니다.");


- 3/17




- rstrip 메서드 오른쪽에 공백이 있을떄 이를 제거해보기
```
data = "039490    "
data = data.rstrip()
print(data)
```
- split 메서드 문자열이 있을떄 btc 와 krw 로 나눔
```
ticker = "btc_krw"
ticker = ticker.split("_")
print(ticker[0])
ticker = "btc_krw"
ticker = ticker.split("_")
print(ticker[1])
```
- split 메서드 공백을 기준으로 문자열 나눔
```
a = "hello world"
a = a.split()
print(a[0])
a = "hello world"
a = a.split()
print(a[1])
```
- capitalize 메서드.앞 단어만 대문자로 변경
```
a = "hello"
a = a.capitalize()
print(a)
```
- 대문자 문자열을 소문자로 변경
```
ticker = "BTC_KRW"
ticker = ticker.lower()
print(ticker)
```
- 소문자 문자열을 대문자로 변경
```
ticker = "btc_krw"
ticker = ticker.upper()
print(ticker)
```

- 3/12

- 좌우의 공백이 있을떄 이를 제거하기
```
data = "    삼성전자    "
data1 = data.strip()
print(data1)
```
- 문자열 슬라이스
```
분기 = "2020/03(E) (IFRS연결)"
print(분기[:7])
```
- 컴마 제거하기
```
상장주식수 = "5,969,782,550"
컴마제거 = 상장주식수.replace(",","")
타입변환 = int(컴마제거)
print(타입변환, type(타입변환))
```
- 이름 나이 출력하는걸 format()메서드 를 사용해서 품
```
name1 = "김민수"
age1 = 10
name2= "이철희"
age2 = 13
print("이름: {} 나이: {}".format(name1, age1))
print("이름: {} 나이: {}".format(name2, age2))
```
- 이름 나이 출력하기

원래 정답
```
name1 = "김민수"
age1 = 10
name2= "이철희"
age2 = 13
print("이름: %s 나이: %d" % (name1, age1))
print("이름: %s 나이: %d" % (name2, age2))
```
내가 쓴 정답
```
name1 = "김민수"
age1 = 10
name2= "이철희"
age2 = 13
print(("이름: 김민수 나이:"),( age1 ));
print(("이름: 이철희 나이:"),( age2 ))
```
- 파이선 자바 더하고 4번- 파이선 자바 더하고 4번 곱하기
```
t1 = 'python'
t2 = 'java'
print(( t1 + " " + t2 + " " ) * 4)
```

- 3/10

- 주소에서 kr만 뺴기
```
url = "http://sharebook.kr"
print(url[-2:])
```
```
url = "http://sharebook.kr"
url_split = url.split('.')
print(url_split[-1])
```
- 전화번호에 - 자 뺴기
```
phone_number = "010-1111-2222"
phone_number1 = phone_number.replace("-"," ")
print(phone_number1)
```
- 홀만 출력하기
```
string = "홀짝홀짝홀짝"
print(string[::2])
```
- 뒤에4자리만 출력
```
license_plate = "24가 2210"
print(license_plate[-4:])
```
- python에서 p t만 출력
```
lang = 'python'
print(lang[0],lang[2])
```
- 15.79를 실수로 
```
data = "15.79"
data = float(data)
print(data, type(data))
```
- 100을 문자열로 변환
```
num = 100
print(str(num))
```
```
num = 100
result = str(num)
print(result,type(result))
```
- 720을 정수로 변환
```
num_str = "720"
print(int(num_str))
```
- 헬로 파이선 더하며 중간에 ! 붙히기
```
s = "hello"
t = "python"
print( s +"!",t )
```

정수 : int
문자열 : str
실수 : float

- 3/8

```
dictionary={
  "name" :"7D 건조 망고",
  "score":10,
  "type":"당절임",
  "ingredient" : ["망고","설탕","메타중아황산나트륨","치자황색소"],
  "orgin":"필리핀"
}

print("name:", dictionary["name"])
print("score:", dictionary["score"])
print("type:", dictionary["type"])
print("ingredient:", dictionary["ingredient"][0])
print("orgin:", dictionary["orgin"])

del dictionary["ingredient"]
print(dictionary)
```

```
dict_a = {
  "name" : "어벤져스 엔드게임",
  
  "type" : "히어로 무비"
}
print(dict_a)
print(dict_a["name"])
```
- 스파이 뺴고 숫자만 
```
list_input_a = ["52","273","32","스파이","103"]
list_a=[]

for i in list_input_a:
  try:
    float(i)
    list_a.append(i)
  except:
    pass

print(list_a)
```
- 원의 반지름,둘레,넓이
```
user_input_a = input("정수입력>")

if user_input_a.isdigit():
  number_input_a = int(user_input_a)

  print("원의 반지름 :", number_input_a)

  print("원의 둘레 :", 2 * 3.14 * number_input_a)

  print("원의 넓이 :", 3.14 * number_input_a * number_input_a)

else:
  print("값이 잘못 입력되었습니다.")
```

- 3/5

- 평균구하기
```
num = [1,2,3,4,5]
print(sum(num)/len(num))
```
- 개수구하기
```
cook = ["피자","김밥","만두"]
print(len(cook))
```
- 합
```
nums = [1,2,3,4,5]
print(sum(nums))
```
- 최대값,최소값
```
nums = [1,2,3,4,5,6,7]
print("max:",max(nums))
print("min:",min(nums))
```
- lang1 lang2 합치기
```
lang1 = ["C","C++","JAVA"]
lang2 = ["Python","Go","C#"]
langs = lang1 + lang2
print(langs)
```
- 뒤에 추가하고 2번쨰에 추가하고 4번쨰꺼 뺴고 3,4번쨰꺼도 빼기
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
