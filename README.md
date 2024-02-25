## 기능명세서
- [x] 참여자 이름을 입력받는다.
  - [x] 쉼표 기준으로 구분한다.
  - [x] 5글자 이하인지 확인한다.
  - [x] 구분자가 연속해서 포함되지 않는다.
  - [x] 구분자로 시작하거나 끝나지 않는 지 확인한다.
  - [x] 공백을 입력하지 않는다.
- [x] 사다리 높이를 입력받는다.
  - [x] 1이상인지 확인한다.
  - [x] 정수인지 확인한다.
  - [x] Integer범위 이내의 숫자인지 확인한다.
- [x] 사다리를 생성한다.
  - [X] 한 층의 다리를 랜덤으로 생성한다.
  - [x] 사다리 높이만큼 생성한다.
  - [x] 사다리의 가로 라인이 겹치지 않도록 생성한다.
- [x] 실행 결과를 출력한다.

## 리팩토링 목록
- [x] 테스트를 클래스 별로 분리하기
- [x] OutputView 메소드 정리하기
- [x] public 메소드 테스트 점검
- [x] 테스트 displayName 추가
- [x] 테스트 내 변수 final 적용
- [x] 이름 중복 검증
- [x] 원시값 포장
- [X] dto 변환
- [X] 일급 컬렉션
- [x] 메소드 10라인
- [x] final: 생성자  (로컬변수) 
- [x] 예외 메시지 작성
- [x] enum 적용
- [x] 예외 발생시 재입력
- [x] outputView 개선 - 커비

## 추가 기능 구현
- [ ] 참여자 이름으로 'all'을 입력받으면 예외 처리한다.
- [ ] 실행 결과를 입력받는다.
  - [x] 쉼표 기준으로 구분한다.
  - [x] 구분자가 연속해서 포함되지 않는다.
  - [x] 구분자로 시작하거나 끝나지 않는 지 확인한다.
  - [x] 공백을 입력하지 않는다.
  - [ ] 실행 결과의 수와 참여자 수가 일치하지 않으면 예외 처리한다.
- [ ] 결과를 보고 싶은 참여자를 입력받는다.
  - [ ] 참여자의 이름을 입력할 시 해당 참여자의 결과만 출력한다.
  - [ ] 'all'을 입력했을 시 전체 참여자의 결과를 출력한다.
  - [ ] 참여자의 이름이나 'all'이 아닌 값을 입력했을 시 예외 처리한다.
- [ ] 종료 시점 고민(예시에선 'all'을 입력한 뒤 종료)

## 고민점
- [ ] 일반 메서드의 파라미터에도 final 키워드가 효과적일까?
- [ ] 같은 맥락으로 컨트롤러의 모든 로컬 변수에 final 붙이는 이유에 대해서도
- [ ] readWithRetry 작동 원리 이해
