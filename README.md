# 로또
## 진행 방법
* 로또 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)


## Step1
### String 클래스에 대한 학습 테스트
#### 요구사항
- `,` 분리 테스트
  - "1,2" 를 `,`로 분리 했을 때 1과 2로 분리되는지 확인
  - "1" 을 `,` 로 분리 했을 때 1만을 포함하는 배열이 반환되는지 확인
- subString 테스트
  - "(1,2)" 를 subString 했을 때에 "1,2" 가 반환되는지 확인
- charAt 테스트
  - "abc" 값이 주어졌을 때, `charAt()` 메소드를 활용해 특정 위치의 문자를 가져오는 학습 테스트를 구현
  - `String`의 `charAt()` 메소드를 활용해 특정 위치의 문자를 가져올 때 위치 값을 벗어나면 `StringIndexOutOfBoundsException`이 발생하는 부분에 대한 학습 테스트를 구현
  - JUnit의 `@DisplayName`을 활용해 테스트 메소드의 의도 표현

### Set Collection에 대한 학습 테스트
#### 요구사항
- Set 의 size() 메소드를 활용해 Set 의 크기 확인
- Set 의 contains() 메소드를 활용해 1, 2, 3 의 값이 존재하는지 확인
  - `@ParameterizedTest`를 활용해 중복 코드 제거
- `@CsvSource`를 활용해 1,2,3 일 때 true, 4,5 일 때 false 반환하는 학습 테스트 구현