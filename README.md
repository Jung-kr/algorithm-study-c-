

## 📙 algorithm-study

* 코딤 테스트 합격자 되기 C++편을 공부한 내용을 저장하는 리파지토리입니다.
* 참고: [코딤 테스트 합격자 되기 C++편(박경록)](https://product.kyobobook.co.kr/detail/S000213087020)

## 🧩Contents

### 1. Array (배열)
[배열 개념](https://velog.io/@jungwy98/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%EB%B0%B0%EC%97%B4)
* 문제 1) [두 수를 뽑아서 더하기*](https://github.com/Jung-kr/algorithm-study-programmers/blob/main/array/problem1)
  * 문제 : https://school.programmers.co.kr/learn/courses/30/lessons/68644
  * set: 중복 허용 X, 자동 정렬
  * set 사용 후 반환 타입인 vector를 맞추기 위해 vector로 변환 
* 문제 2) [모의고사*](https://github.com/Jung-kr/algorithm-study-programmers/blob/main/array/problem2)
  * 문제: https://school.programmers.co.kr/learn/courses/30/lessons/42840
  * (중복시 정렬하여)최대값의 인덱스 구하는 방법
  * int max = *max_element(correctCnt.begin(), correctCnt.end());  //컨테이너(vector, set, map...) 내에서 최대값
* 문제 3) [행렬의 곱셈*](https://github.com/Jung-kr/algorithm-study-programmers/blob/main/array/problem3)
  * 문제: https://school.programmers.co.kr/learn/courses/30/lessons/12949
  * 2차원 벡터에 접근하기 위해서는 필요한 영역을 미리 할당해줘야 함  //vector<vector<int>> answer; -> answer[i][k] += ...//접근 불가능
  * vector<vector<int>> answer(arr1.size(), vector<int>(arr2[0].size(), 0));  //arr1의 행, arr2의 열 크기를 가진 2차원 벡터 answer 
* 문제 4) [실패율** ]()
  * 문제: 
* 문제 5) [방문길이**](https://github.com/Jung-kr/algorithm-study-programmers/blob/main/array/problem5)
  * 문제: https://school.programmers.co.kr/learn/courses/30/lessons/49994
  * 2차원 공간에서의 방향 벡터 문제 기본 세팅
  * 2차원 공간에서의 중복 -> 3차원 배열 사용 bool check[11][11][4];  //[x좌표][y좌표][방향 인덱스]가 true or false

--- 

### 8. Hash (해시)
[해시 개념](https://velog.io/@jungwy98/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%ED%95%B4%EC%8B%9C) 
`unordered_set`, `unordered_map` 은 내부 구조가 해시 기반이기 때문에 **삽입**, **삭제**, **탐색**의 시간 복잡도가 **O(1)** 
* 문제(기초) 1) [두 개의 수로 특정 값 만들기*](https://github.com/Jung-kr/algorithm-study-programmers/blob/main/hash/problem1)
  * 해시 개념에 대한 기본 문제, vector로 해시 구축
  * O(1)으로 데이터 접근이 필요할 때 -> 미리 데이터로 해시를 구축하 배열 인덱스로 접근
