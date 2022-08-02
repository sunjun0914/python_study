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
