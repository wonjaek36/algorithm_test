Category
* Greedy

Solved
* 세 수를 뽑았을 때, 크기 순으로 A, B, C라고 하자
  * 이 때, 값으로 구해야 하는 것은 (A + B + C) - B * 3 = (A + C) - B * 2
  * 식을 조금 변경해보면, abs( (C-B) - (B-A) ) 의 최대값을 구하는 문제로 바뀐다
  * A, B, C를 수직선 상에 그려놓고 보면,
    * A, B는 최대한 가깝고, C는 최대한 먼 것이 유리
    * 따라서, 숫자 A를 정했을 때, B와 C가 정해진다. O(N)
      * B를 C에 최대한 가깝게 하는 경우도 고려해야함.
