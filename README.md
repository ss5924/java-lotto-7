# java-lotto-precourse

## 가. 기능 요구 사항

#### 간단한 로또 발매기를 구현한다.

- [x] 로또 번호의 숫자 범위는 1~45까지이다.
- [x] 1개의 로또를 발행할 때 중복되지 않는 6개의 숫자를 뽑는다.
- [x] 당첨 번호 추첨 시 중복되지 않는 숫자 6개와 보너스 번호 1개를 뽑는다.
- [x] 당첨은 1등부터 5등까지 있다. 당첨 기준과 금액은 아래와 같다.
    - 1등: 6개 번호 일치 / 2,000,000,000원
    - 2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
    - 3등: 5개 번호 일치 / 1,500,000원
    - 4등: 4개 번호 일치 / 50,000원
    - 5등: 3개 번호 일치 / 5,000원
- [x] 로또 구입 금액을 입력하면 구입 금액에 해당하는 만큼 로또를 발행해야 한다.
- [x] 로또 1장의 가격은 1,000원이다.
- [x] 당첨 번호와 보너스 번호를 입력받는다.
- [x] 사용자가 구매한 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 출력하고 로또 게임을 종료한다.
- [x] 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시키고, "[ERROR]"로 시작하는 에러 메시지를 출력 후 그 부분부터 입력을 다시 받는다. Exception이 아닌
  IllegalArgumentException, IllegalStateException 등과 같은 명확한 유형을 처리한다.


## 나. 개발 plan

1. Lotto
   - [x] lotto 번호 validation check 및 저장 구현
2. LottoGenerator
   - [x] lotto 번호 랜덤 생성 기능 개발
3. LottoShop
   - [x] 구매 금액에 따라 lotto 발행 
4. LottoChecker
   - [x] 발급된 랜덤번호와 당첨 번호 비교
   - [x] 보너스 번호 validation check 
5. LottoStatistics
   - [x] 당첨 내역 집계
   - [x] 수익률 계산
6. LottoPrinter
   - [x] 결과 출력 형식 관리
7. InputValidator
   - [x] 입력 프로세스 구현
   - [x] 잘못된 입력값 validation check 하여 해당 부분부터 재입력
8. Application
   - [x] 입출력 프로세스 구현