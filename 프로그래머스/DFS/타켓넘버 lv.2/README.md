# <a href="https://school.programmers.co.kr/learn/courses/30/lessons/43165">타켓 넘버</a>

### 문제 설명
<p>n개의 음이 아닌 정수들이 있습니다. 이 정수들을 순서를 바꾸지 않고 적절히 더하거나 빼서 타겟 넘버를 만들려고 합니다. 예를 들어 [1, 1, 1, 1, 1]로 숫자 3을 만들려면 다음 다섯 방법을 쓸 수 있습니다.
<pre>
-1+1+1+1+1 = 3
+1-1+1+1+1 = 3
+1+1-1+1+1 = 3
+1+1+1-1+1 = 3
+1+1+1+1-1 = 3
</pre>
사용할 수 있는 숫자가 담긴 배열 numbers, 타겟 넘버 target이 매개변수로 주어질 때 숫자를 적절히 더하고 빼서 타겟 넘버를 만드는 방법의 수를 return 하도록 solution 함수를 작성해주세요.</p>

### 제한사항
<ul>
<li>주어지는 숫자의 개수는 2개 이상 20개 이하입니다.</li>
<li>각 숫자는 1 이상 50 이하인 자연수입니다.</li>
<li>타겟 넘버는 1 이상 1000 이하인 자연수입니다.</li>
</ul>

### 입출력 예
<table>
<th>numbers</th>
<th>target</th>
  <th>return</th>
  <tr>
<td>[1, 1, 1, 1, 1]</td>	
<td>3</td>	
    <td>5</td>
</tr>
  <tr>
<td>[4, 1, 2, 1]</td>	
    <td>4</td>
     <td>2</td>
  </tr>
</table>


### 문제 해결 과정

<pre>
 
완전탐색은 테스트 케이스의 최악의 경우에 몇번의 연산을 해야하는 지 계산해본다.
500만번 미만이면 가능하다.
최대 20개의 숫자, 2가지의 경우
2^20은 백만번정도이다.

</pre>

