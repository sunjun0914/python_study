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
# python study

## 2022-08-04

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

data = [2, 4, 3, 1, 5, 10, 9]
data.sort()
print(data)
(data를 오름차순으로 정렬)

data = [2, 4, 3, 1, 5, 10, 9]
data2 = sorted(data)
print(data2)
(data2에 data를 오름차순으로 정렬한 것을 저장)
```






















