Diagonal Differenc
=======

언어 : Python3

난이도 : Easy

문제 : 주어진 배열의 좌우 각 대각선의 합의 차를 구하라

코드

<pre><code> def diagonalDifference(arr):
    
    left = 0
    right = 0
    
    for i in range(len(arr)):
        left = left + arr[i][i]
        right = right + arr[i][-(i + 1)]
        
    return abs(left - right) </code></pre>


풀이 : 행렬의 좌표 (0,0) 부터 차례대로 정방으로 합을 구하고 역으로 합을 구하기로함

계산은 맞았는데 출력값이 달라서 뭐가 문제인지 보다가 값이 음수가 아닌 절대값을 구해야 한다는것을 확인

절대값은 어떻게 구하는것인가 검색 결과 abs함수를 사용한다는 것을 알게 되었고 간단히 해결


abs
-----
전달한 숫자의 절대값을 반환 plain integer, long integer, float point number 등의 숫자를 argument로 넘겨주면 절대값을 반환

만약 복소수를 argument로 넘겨주면 복소수의 크기(magnitude)를 결과로 반환
