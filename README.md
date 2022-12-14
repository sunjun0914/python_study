# python_study

## 2022-08-02
- 문자열을 입력받아 거꾸로 출력하는 프로그램
```python
outStr =""
count, i = 0,0

inStr =input("Type string: ")
count = len(inStr)

for i in range(0,count) :
    outStr += inStr[count - (i+1)]

print("Reversed string : %s" % outStr)
```

- 문자열 구성 파악 함수
```
isdigit():문자열이 숫자인가?
isalpha():문자열이 문자인가?
isalnum():문자열이 문자+숫자 혼합인가?
isupper():문자열이 대문자인가?
islower():문자열이 소문자인가?
isplace():문자열이 공백인가?
```

- 대소문자 변환 함수
```
upper():대문자로 변환
lower():소문자로 변환
swapcase()대소문자 상호 변환
title()단어의 첫 글자를 대문자로 변환
```
- 문자열 찾기 함수
```
count('a'):문자열에서 'a'개수
find('a'):문자열에서 'a'의 처음위치. 없으면 -1 반환
rfind('a'):문자열에서 'a'가 나오는 가장 마지막위치(오른쪽부터 처음위치). 
index('a'):문자열에서 'a'의 처음위치. 없으면 ValueError
```

# 2022-08-04

- 리스트에서 최대값과 최소값 출력하기

```
max:최대값을 구하는 함수
min:최소값을 구하는 함수

nums = [1, 2, 3, 4, 5]
print("max:",max(nums))
print("min:",min(nums))

출력결과
max:5
min:1
```

- 리스트의 합 출력하기

```
sum:합계를 구하는 함수

nums = [1, 2, 3, 4, 5]
print(sum(nums))

출력결과
15
```

- 리스트에 저장된 데이터의 개수 출력하기
```
len:데이터의 개수를 세는 함수

food = ["피자", "치킨", "떡볶이", "햄버거", "김밥", "라면","만두"]
print(len(food))

출력결과
7
```

- 리스트의 평균 출력하기

```
평균 구하는 방법: 리스트의 합(sum) / 리스트의 개수(len)

nums:[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
nums2 = sum(nums) / len(nums)
print(nums2)

출력결과
5.5
```

- 슬라이싱을 이용한 수 출력

```
print(변수[시작:끝:간격])

-날짜정보를 제외한 가격 정보만 출력

price = ['20180728', 100, 130, 140, 150, 160, 170]
print(price[1:])

-1~10중 홀수,짝수만 출력
nums = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
홀수 : print(nums[::2])
짝수 : print(nums[1::2)

-역방향으로 출력
nums = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(nums[::-1])

-일부만 출력
subject = ['국어', '수학', '영어']
print(interest[0],interest[2])
출력결과: 국어 영어
```

- join 메서드 
```
interest = ['삼성전자', 'LG전자', 'Naver', 'SK하이닉스', '미래에셋대우']
print(" ".join(interest))
출력결과
삼성전자 LG전자 Naver SK하이닉스 미래에셋대우

print("/".join(interest))
출력결과
삼성전자/LG전자/Naver/SK하이닉스/미래에셋대우

print("\n".join(intrest))
출력결과
삼성전자
LG전자
Naver
SK하이닉스
미래에셋대우
```

- split 메서드 

```
string = "삼성전자/LG전자/Naver"
interest = string.split("/")
print(interest)
실행결과
['삼성전자', 'LG전자', 'Naver']
```

-리스트 정렬

```

data = [2, 4, 3, 1, 5, 10, 9]
data.sort()
print(data)
(data를 오름차순으로 정렬)

data = [2, 4, 3, 1, 5, 10, 9]
data2 = sorted(data)
print(data2)
(data2에 data를 오름차순으로 정렬한 것을 저장)

```

# 2022-08-09

- 튜플 생성및저장
```
-튜플 생성
my_variable = ()
print(type(my_variable))
괄호는 튜플을 정의하는 기호

-영화 제목을 튜플에 저장
movie = ("탑건","닥터스트레인지","토르","미니언즈")

-숫자가 저장된 튜플 생성
number = (1)
type(number)

-원칙적으로 튜플은 괄호와 함께 데이터를 정의해야 하지만, 사용자의 편의의 따라 괄호없이도 동작 가능
t = 1, 2, 3, 4
```

- 튜플 변환
```
-('a','b','c')가 입력된 변수 t가 ('A','b','c')튜플을 가리키도록 수정
(튜플의 값은 변경이 불가해  t[0] = 'A'  과 같은 코드는 동작이 불가능,변수를 업데이트 해야됨)

t = ('a','b','c')
t = ('A','b','c')

-튜플을 리스트로 변환

interest = ('삼성전자','LG전자','SK Hynix')
interest_list = list(interest)
type(interest_list)

-리스트를 튜플로 변환

interest = ('삼성전자','NAVER','SK하이닉스')
interest_tuple = tuple(interest)
type(interest_tuple)
```

- range함수(정수 생성)
```
-1부터 99까지의 정수중 짝수만 저장된 튜플 생성
number = tuple(range(2,100,2))
print(number)

-1부터 99까지의 정수중 홀수만 저장된 튜플 생성
number = tuple(range(1,100,2))
print(number)
```
# 2022-08-11

- 딕셔너리 만들기
```
- 딕셔너리 = {키1:값1,키2:값2}
lucian = {'health':490,'mana':334,'melee':550,'armor':18.72)
```
- dick로 딕셔너리 만들기
```
-딕셔너리 = dick()

- 딕셔너리 = dick(키1=값1,키2=값2)
lucian1 = dict(health=490,mana=334,melee=550,armor=18.72)
lucian1

- 딕셔너리 = dick(zip([키1,키2],[값1,값2]))
lucian2 = dict(zip(['health','mana','melee','armor'],[490,334,550,18.72))
lucian2

- 딕셔너리 = dick([(키1,값1)],[(키2,값2)])
lucian3 = dick([(health,550),(mana,334),(melee,550),(armor,18.72)])
lucian3

- 딕셔너리 = dick({키1:값1,키2:값2})
lucian4 = dick({'health':550,'mana':334,'melee':550,'armor':18.72})
lucian4

실행결과
{'health': 490, 'mana': 334, 'melee': 550, 'armor': 18.72}
```
- 딕셔너리에 접근하고 값 할당하기
```
lucian = {'health':490,'mana':334,'melee':550,'armor':18.72}
lucian['health']
실행결과
490
lucian['armor']
18.72

*딕셔너리에 키를 저장하지 않으면 헤당 딕셔너리 전체를 뜻함
```
- 딕셔너리의 키의 값 할당하기
```
lucian = {'health':490,'mana':334,'melee':550,'armor':18.72}
lucian['health'] = 2037
lucian['mana'] = 2399
lucian

실행결과
{'health':2037 'mana':2399,'melee':550,'armor':18.72}

lucian = {'health':490,'mana':334,'melee':550,'armor':18.72}
lucian['mana_regen'] = 3.66
lucian
실행결과
{'health':490,'mana':334,'melee':550,'armor':18.72,'mana_regen':3.66}
```

- 딕셔너리에 키가 있는지 확인
```
lucian = {'health':490,'mana':334,'melee':550,'armor':18.72}
'health' in lucian
결과: True
'attack_speed'in lucian
결과: False
'health' not in lucian
결과: False
'attack_speed' not in lucian
결과: True
```
# 2022-08-18
- if 조건문
```
if 조건식:
    코드
만약 조건식이 참이라면 코드를 실행한다
 x = 10
 if x == 10:]
    print('10입니다.')
  
 결과: 10입니다
```
- if 조건문 들여쓰기
```
x = 10 
if x == 10:
    print('x에 들어있는수는')
        print('10입니다')
       
오류발생
옳은코드
x = 10 
if x == 10:
    print('x에 들어있는수는')
    print('10입니다')
  
결과:x에 들어있는수는 10입니다
해설:두번째 print도 4칸 들여쓰기를 해야됨

x = 5
if x == 10:
    print('x에 들어가있는 숫자는')
print('10입니다')

결과:10
해설:조건에 맞지 않기 때문에 두번째 print로 넘어가서 10입니다만 출력됨
```
- 중첩된 if 조건문
``` 
x = 15
if x >= 10:
    print('10이상입니다.')
    if x == 15:
        print('15입니다.')
    if x == 20:
        print('20입니다.')
        
결과: 10이상입니다.
      15입니다.
해설:들여쓰기를 보면 첫번째 if문에 두번째,세번째 if문이 포함되어있다
첫번째 if문이 참이므로 두번째,세번째 if문도 확인한다
두번째 if문은 참,세번째 if문은 거짓이므로 첫번째와 두번째 if문만 실행되었다
```
- 입력받은 값에 if문 사용하기
```
x = int(input))
if x == 10:
    print('10입니다')
if x == 20:
    print('20입니다')

입력:10
결과:10입니다
입력:20
결과:20입니다
입력:5
결과없음
```
# 2022-08-23
- elif 사용
```
형식:
if 조건식:
    코드1
elif 조건식:
    코드2
예시)
x = 10
if x == 10
    print('10입니다')
elif x == 20
    print('20입니다')
결과:10입니다
```
- if,elif,else 모두 사용
```
형식
if 조건식:
    코드1
elif 조건식:
    코드2
else 조건식:
    코드3
예시)
x = 30
if x == 10:
    print('10입니다')
elif x == 20:
    print('20입니다')
else:
    print('10 또는 20이 아닙니다')
결과:10또는 20이 아닙니다
```
- 값 입력받아 결과 출력
```
x = int(input())
if 1 <= x <= 10 :
    print('1~10')
elif 11<= x <= 20:
    print('11~20')
else('아무것도 해당하지 않음')
입력:9 -> 결과:1~10
입력:13 -> 결과:11~20
입력:31 -> 결과:아무것도 해당되지않음
-음료수 자판기 만들기
button = int(input())
if button == 1:
    print('콜라')
elif button == 2:
    print('사이다')
elif button == 3:
    print('환타')
else:
    print('제공하지 않는 음료')
   
입력:1 -> 결과:콜라
입력:2 -> 결과:사이다
입력:3 -> 결과:환타
입력:4 -> 결과:제공하지 않는 음료
```
-for와 range 사용
형태:
for 변수 in range(횟수):
    반복할 코드
예시)
for i in range 100:
    print(Hi,i)














































































































































































































