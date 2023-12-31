# <a href="https://school.programmers.co.kr/learn/courses/30/lessons/42587">프로세스 </a>

### 문제 설명
<p>운영체제의 역할 중 하나는 컴퓨터 시스템의 자원을 효율적으로 관리하는 것입니다. 이 문제에서는 운영체제가 다음 규칙에 따라 프로세스를 관리할 경우 특정 프로세스가 몇 번째로 실행되는지 알아내면 됩니다.
  <pre>
1. 실행 대기 큐(Queue)에서 대기중인 프로세스 하나를 꺼냅니다.
2. 큐에 대기중인 프로세스 중 우선순위가 더 높은 프로세스가 있다면 방금 꺼낸 프로세스를 다시 큐에 넣습니다.
3. 만약 그런 프로세스가 없다면 방금 꺼낸 프로세스를 실행합니다.
  3.1 한 번 실행한 프로세스는 다시 큐에 넣지 않고 그대로 종료됩니다.
예를 들어 프로세스 4개 [A, B, C, D]가 순서대로 실행 대기 큐에 들어있고, 우선순위가 [2, 1, 3, 2]라면 [C, D, A, B] 순으로 실행하게 됩니다.

현재 실행 대기 큐(Queue)에 있는 프로세스의 중요도가 순서대로 담긴 배열 priorities와, 몇 번째로 실행되는지 알고싶은 프로세스의 위치를 알려주는 location이 매개변수로 주어질 때, 해당 프로세스가 몇 번째로 실행되는지 return 하도록 solution 함수를 작성해주세요.  </pre></p>

### 제한사항
<ul>
<li>priorities의 길이는 1 이상 100 이하입니다.</li>
<li>priorities의 원소는 1 이상 9 이하의 정수입니다.</li>
<li>priorities의 원소는 우선순위를 나타내며 숫자가 클 수록 우선순위가 높습니다.</li>
<li>location은 0 이상 (대기 큐에 있는 프로세스 수 - 1) 이하의 값을 가집니다.</li>
<li>priorities의 가장 앞에 있으면 0, 두 번째에 있으면 1 … 과 같이 표현합니다.</li>
</ul>
### 입출력 예
<table>
<th>priorities	</th>
<th>location</th>
  <th>return</th>
  <tr>
<td>[2, 1, 3, 2]</td>	
  <td>2</td>
    <td>2</td>
</tr>
  <tr>
<td>[1, 1, 9, 1, 1, 1]</td>	
    <td>0</td>
     <td>5</td>
  </tr>
</table>

### 입출력 예 설명
<p>
<ul>
예제 #1
<li>문제에 나온 예와 같습니다.</li>
<br>
예제 #2
<li>6개의 프로세스 [A, B, C, D, E, F]가 대기 큐에 있고 중요도가 [1, 1, 9, 1, 1, 1] 이므로 [C, D, E, F, A, B] 순으로 실행됩니다. 따라서 A는 5번째로 실행됩니다.</li>
</ul>
</p>
  
### 문제 해결 과정

<pre>
 
*for( int i : A )
A에서 차례대로 객체를 꺼내서 i에다가 넣는다.
A에 더이상 꺼낼 객체가 없을 때 까지

*A.stream().anyMatch() A에서 하나씩 꺼내서 충족하는 게 있는지 확인한다. 

</pre>
