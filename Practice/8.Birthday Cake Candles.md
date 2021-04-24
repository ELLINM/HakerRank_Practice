Birthday Cake Candles
======

언어 : Python3

난이도 : Easy

문제 : 주어진 배열의 최대값의 갯수를 구하라

코드

<pre><code>def birthdayCakeCandles(candles):
    max_value = max(candles)
    num = candles.count(max_value)
    return num</code></pre>
    
풀이 : 최대값을 넣을 변수를 생성하고 다시 최대값의 개수를 넣을 변수를 생성한 후 반환

풀고나서 보니 더 짧게 하려면 충분히 할 수 있는거 같다 머리를 좀 써야겠다
