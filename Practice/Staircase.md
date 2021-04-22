Staircase
=====

언어 : Python3

난이도 : Easy

문제 : 입력되는 숫자만큼의 줄에 차례대로 '#'을 출력

코드

<pre><code>def staircase(n):
    for i in range(n):
        for j in range(n):
            if j < n - i - 1:
                 print(" ", end='')
            else:
                print("#", end='')
        print()</code></pre>
        
풀이 : 흔히들 하는 별찍기 첫번째 줄부터 차례대로 For문을 돌려가면서 출력하면
