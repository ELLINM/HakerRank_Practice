Plus Minus
=======

언어 : Python3

난이도 : Easy

믄제 : 입력되는 배열에서 양수, 음수, 0의 비율을 구하라

코드

<pre><code>def plusMinus(arr):
    pn = 0
    nn = 0
    zero = 0
    for i in range(len(arr)):
        if arr[i] > 0:
            pn = pn + 1
        elif arr[i] < 0:
            nn = nn + 1
        else:
           zero = zero + 1
    
    len_arr = len(arr)
    pnf = pn/len_arr
    nnf = nn/len_arr
    zerof = zero/len_arr
    
    print(pnf)
    print(nnf)
    print(zerof)</code></pre>
    
풀이 : For문으로 배열의 수 하나씩 양수, 음수, 0일경우를 따져 각각저장하고 배열의 길이로 나눠서 비율을 구한다
