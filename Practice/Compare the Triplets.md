Compare the Triplets 풀이
=========

언어 : Python3

난이도 : Easy

문제 : 두개의 각 배열의 수를 차례대로 비교하여 스코어를 부여하여 출력

코드

<pre><code>import math
import os
import random
import re
import sys

# Complete the compareTriplets function below.
def compareTriplets(a, b):
    
    ac = 0
    bc = 0
    
    for i in range(len(a)):
        if a[i] > b[i]:
            ac += 1
        elif a[i] < b[i]:
            bc += 1
        elif a[i] == b[i]:
            pass
    return ac, bc    </code></pre>
    
    
풀이 : for문을 돌려서 비교해야한다는건 인지 했으나 a, b 두개를 같이 돌려야하나
많은 헷갈렸음 그러다 re 모듈을 보고 사용할 방법이 있을까 찾아보다가 내머리로는 생각이 안나서
For문에 대한 기억과 설명을 생각하고 차례대로 비교하는 방법을 골라서 풀었다

re
-----
정규표현식(Regular expression)을 이용한 문자열 매칭에 사용되는 파이썬 라이브러리
파이썬 정규표현식을 이용하여 문자열에서 특정 패턴의 문자열을 매칭하는 기능을 제공
정규표현식은 '.', '*', '$' 등의 특수한 메타문자를 이용
더 자세한 설명은 파이썬 정규표현식을 참고


- 제공하는 기능

>re.compile()
정규식 패턴을 파이썬이 사용할 수 있는 정규식 객체로 컴파일 해주는 기능
re.compile()을 통해 객체로 변환된 정규식은 match()와 search()를 통해 검색할 때 패턴으로 이용

>re.search() #
re.compile()을 통해 객체로 변환된 패턴을 받아 문자열에서 패턴을 검색하는 기능
반환값은 매칭 정보를 가지고 있는 re모듈의 Match object
문장전체에서 패턴과 일치하는 부분을 검색

>re.match() #
re.search()와 비슷하나 문장처음부터 패턴과 일치하는 문자열만 검색하는 기능
반환값은 Match objects

>re.findall() #
search나 match는 문자열에서 패턴과 일치하는 첫번째 문자열만 반환해 주지만
re.findall()을 사용하면 문자열에서 패턴과 일치하는 모든 문자열을 리스트형태로 반환

>re.finditer() #
문자열에서 패턴과 일치하는 모든 문자열의 Match object를 iteration할 수 있게 해줌


range
------
for문과 함께 자주 사용되는 함수로 입력받은 숫자에 해당하는 범위의 값을 반복 가능한 객체로 만들어 리턴


len()
-----
입력값의 길이(요소의 전체 개수)를 리턴하는 함수
