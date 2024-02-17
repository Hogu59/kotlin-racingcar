# kotlin-racingcar

## 🏎 ️자동차 경주

 - [x] 자동차 입력 문구 출력
 - [x] 자동차 이름 입력
 - [x] 시도 횟수 입력 문구 출력
 - [x] 시도 횟수 입력
 - [x] 실행 결과 헤더 출력
 - [x] 전진 조건 판단 구현 (1~9 사이 임의 숫자 4 이상인 경우 전진)
 - [x] 각 회차별 결과 출력
 - [x] 최종 우승자 판별 구현
 - [x] 최종 우승자 결과 출력

### 예외 (Car)
 - [x] 차 한대 입력시
 - [x] 이름 길이가 1 미만, 5초과인 경우
 - [x] 자동차 숫자는 2~20대 사이만 가능
 - [x] 입력이 공백인 경우
 - [x] 같은 이름이 있는 경우
 - [x] 이름 안에 공백이 있는 경우

### 예외 (Round Number)
- [x] 숫자가 1보다 작을 때
- [x] Integer 범위를 초과할 경우
- [x] 입력값이 공백일 때


### 수정해야 할 사항 (Need to be fixed)
- [ ] RaceTest ERROR FIX
  - Due to change of companion object of Race class.
- [ ] WinnerTest ERROR FIX
  - Two functions are referencing different scope.
  - getWinners function is using parameter to access "cars".
  - judgeWinners function is using class memeber variable to access "cars".
- [ ] Seperate Validation class
  - To validate the input data globally, it seems seperating validation class reasonable.
- [ ] Function block lines reduction needed.
  - All function block lines should be less than 15.
- [ ] Make private if there is no access from outside.
- [ ] `assertEquals` -> `assertThat` modify.
- [ ] Erase unnecessary companion objects.
  - As Validation class already use the constants, some constants became unnecessary.
- [ ] Depth Reduction needed.
  - All depth should be 1.