
## <a href="https://school.programmers.co.kr/learn/courses/30/lessons/42577?language=java">전화번호 목록</a>

### 문제 설명
<p>전화번호부에 적힌 전화번호 중, 한 번호가 다른 번호의 접두어인 경우가 있는지 확인하려 합니다.
전화번호가 다음과 같을 경우, 구조대 전화번호는 영석이의 전화번호의 접두사입니다.

<ul>
<li>구조대 : 119</li>
<li>박준영 : 97 674 223</li>
<li>지영석 : 11 9552 4421</li>
<li>전화번호부에 적힌 전화번호를 담은 배열 phone_book 이 solution 함수의 매개변수로 주어질 때, 어떤 번호가 다른 번호의 접두어인 경우가 있으면 false를 그렇지 않으면 true를 return 하도록 solution 함수를 작성해주세요.</li>
</ul>
</p>

### 제한 사항
<p>
    phone_book의 길이는 1 이상 1,000,000 이하입니다.
각 전화번호의 길이는 1 이상 20 이하입니다.
같은 전화번호가 중복해서 들어있지 않습니다.
</p>

### 입출력 예제
<table>
    <th>phone_book</th>
	<th>return</th>
    <tr>
        <td>["119", "97674223", "1195524421"]</td>
        <td>false</td>
    </tr>
<tr>
    <td>["123","456","789"]</td>
    <td>true</td>
</tr>
<tr>
    <td>["12","123","1235","567","88"]</td>
    <td>false</td>
</tr>
</table>
        
### 입출력 예 설명
<ul>
입출력 예 #1
<li>앞에서 설명한 예와 같습니다.</li>

입출력 예 #2
<li>한 번호가 다른 번호의 접두사인 경우가 없으므로, 답은 true입니다.</li>
<br>
입출력 예 #3
<li>첫 번째 전화번호, “12”가 두 번째 전화번호 “123”의 접두사입니다. 따라서 답은 false입니다.</li>
</ul>

### 문제 해결 과정

<ol>
<li> sort 후</li>
    array.startsWith(answer); // array 배열이 answer로 시작하는지 확인하는 함수
<li> hash 사용</li>
</ol>


