# 자동차 경주 게임
## 진행 방법
* 자동차 경주 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

## 구현할 기능 목록
- [ ] "경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)\n" 텍스트 출력
- [ ] 유저가 입력한 [자동차 이름]을 ',' 단위로 파싱해서 Struct Car를 담고 있는 배열에 저장 (`IllegalArgumentException` 감지 필요, Struct Car는 String [자동차 이름], Int [전진한 칸] 으로 이루어져 있음)
- [ ] "시도할 횟수는 몇회인가요?\n" 텍스트 출력
- [ ] 유저가 입력한 [시도할 횟수]를 int로 저장 (`IllegalArgumentException` 감지 필요)
- [ ] "\n실행 결과\n" 텍스트 출력
- [ ] 각 자동차마다 0~9 무작위 값 generate한 뒤, 4 이상이면 전진한 칸을 1 증가시킴. (C++이라면 for문 돌리겠지만, Kotlin은 다른 방법 있나 찾아보기 - 왠지 있을 것 같음, 무작위 값은 굳이 int일 필요없어보임. 전진한 칸 수는 int로 저장)
- [ ] 각 자동차마다 "${자동차 이름} : ", 전진한 칸 수 만큼 '-', '\n'을 출력.
- [ ] 모든 자동차마다 전진한 칸 수 출력이 끝났으면 '\n'을 출력.
- [ ] [시도할 횟수] 변수 1 감소
- [ ] [시도할 횟수] 변수가 0이 되었다면, "\n최종 우승자 : " 텍스트 출력.
- [ ] Car 배열에서 [전진한 칸]이 가장 많은 Car의 [자동차 이름]을 출력. 이 때, 각 [자동차 이름]사이에 ", "를 넣어서 출력한다. (왠지 Kotlin의 람다함수를 잘 이용하면 이 과정을 한줄로 만들 수 있을 것 같음)
