## 🔍 동작 구분
1. 게임을 시작한다.
2. 컴퓨터(상대방) 이 랜덤한 3자리 수를 생각한다.
   1. 각 자리가 중복된 수가 없도록 체크 후 넣는다.
3. 유저(플레이어) 가 3자리 숫자를 입력한다.
   1. 각 자리가 중복된 수가 없는지 체크 후 있다면 오류를 반환하고, 없다면 추가한다.
   2. 각 자리 입력자가 숫자인지 파악 후 문자라면 오류를 반환하고, 숫자라면 추가한다.
   3. 유저가 총 입력한 문자들이 3글자인지 확인 후 3글자가 아니라면 오류를 반환하고, 맞다면 추가한다.
4. 컴퓨터가 생각한 3자리 숫자와 유저가 입력한 3자리 숫자를 비교한다.
5. 두 숫자의 위치와 숫자가 일치한다면 스트라이크, 숫자만 일치하고 위치는 일치하지 않다면 볼, 아무것도 일치하지 않는다면 아무것도 반환하지 않는다.
6. 5번의 결과물들 3가지를 종합 후 스트라이크, 볼 횟수를 반환한다. 만약 아무것도 오지 않는다면 낫싱을 반환한다.
7. 3~6번의 과정을 3스트라이크가 나올때까지 반복한다.
8. 만약 3스트라이크가 나오면 유저에게 게임을 재실행할지 물어본다.
   1. 1번이라면 재시작, 2번이라면 종료, 그 외의 문자라면 재입력을 받는다.


## 🚀 기능 목록

1. 컴퓨터의 랜덤 수 생성하기.
2. 1번에서 생성한 수와 컴퓨터 입력값 배열 요소들간의 중복 체크하기.
3. 1~2번의 과정을 컴퓨터 입력값 배열의 길이가 3이 될 때 까지 반복하기.
4. 유저에게 3자리의 입력값 받기.
5. 4번에서 받은 값의 길이가 3글자가 맞는지 판단하기.
6. 4번에서 받은 값이 전부 숫자인지 판단하기.
7. 4번에서 받은 값에 중복된 숫자가 있는지 판단하기.
8. 만약 5~7번의 과정에서 예외사항이 있다면 오류를 반환하고 종료하기.
9. 컴퓨터가 입력한 3글자와 유저가 입력한 3글자를 비교하기.
10. 만약 숫자와 배열 내부에서의 위치가 일치한다면 스트라이크 카운트를 1 올리기.
11. 만약 숫자만 일치하고 배열 내부에서의 위치가 다르다면 볼 카운트를 1 올리기.
12. 10번, 11번의 과정에서 스트라이크와 볼 카운트를 종합 후 결과 반환하기.
13. 만약 스트라이크와 볼이 전부 0이라면 낫싱 반환하기.
14. 4~13의 과정을 스트라이크 카운트가 3이 될 때까지 반복하기.
15. 만약 스트라이크 카운트가 3이라면 게임을 재시작할지 여부 확인하기.
16. 유저가 1을 입력했다면 1~15번의 과정을 다시 반복하고, 2를 입력했다면 종료하기.
17. 만약 유저가 1이나 2가 아닌 다른 문자를 입력했다면 재입력받기.