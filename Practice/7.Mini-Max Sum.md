Mini-Max Sum
=======

언어 : Python3

난이도 : Easy

문제 : 주어진 배열의 합을 구하라 단, 배열의 수중 하나씩 제외하여 합을 구하고 합중에서 최대값과 최소값을 출력하라

코드

<pre><code>def miniMaxSum(arr):
    arr_sum = sum(arr)
    arr_max = max(arr)
    arr_min = min(arr)
    
    print(arr_sum - arr_max, arr_sum - arr_min)</code></pre>

풀이 : 처음에는 배열의 수를 하나씩 빼가며 비교해야하는지 생각 했다가 단순하게 배열의 총합에서 배열의 최대값과 최소값을 빼면

쉽다는걸 깨달았다. 
