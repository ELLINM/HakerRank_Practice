Simple Array Sum 풀이
=======

언어 : Python3

난이도 : Easy

문제 :  주어진 정수 배열의 합을 구하라


코드
<pre><code>def simpleArraySum(ar):
    return sum(ar)</code></pre>


풀이 : 처음에는 배열 For문을 돌리면서 하나씩 더해야하나 했음 

그러다가 파이썬 배열 합을 구글링 해본 결과 간단한 함수 하나면 끝나는걸 알게됨


sum
-----

>start 및 iterable 의 항목들을 왼쪽에서 오른쪽으로 합하고 합계를 돌려줍니다. 
 iterable 의 항목은 일반적으로 숫자며 시작 값은 문자열이 될 수 없습니다.
 어떤 경우에는 sum() 에 대한 좋은 대안이 있습니다. 문자열의 시퀀스를 연결하는 가장 선호되고 빠른 방법은 ''.join(sequence) 를 호출하는 것입니다. 
 확장된 정밀도로 부동 소수점 값을 더하려면 math.fsum() 를 보세요. 일련의 이터러블들을 연결하려면 itertools.chain() 를 고려해보세요.

위는 함수에대한 설명이다.

