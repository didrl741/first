# gitHub 사용법

## 안녕하세요

- clone : repo 복사
- add : 스테이지에 올리기
- commit : 세이브. 스테이지 영역의 파일들을 세이브할 수 있다.
- push : 원격 저장소에 커밋을 업로드.


## 브랜치 변경하기

- 브랜치란 : 기존 내용을 유지한 채, 새로운 내용을 추가하고 싶을 때 사용.
- 체크아웃 : 특정 브랜드(커밋)으로 돌아가고 싶을 때 사용.
- 소스트리의 체크아웃 : 브랜치 이름을 더블클릭.

## 병합하기 1

- 헤드 브랜치에 변경사항이 없고
- 병합 대상 브랜치가 헤드로부터 시작된 경우
- 아주 쉽게 병합 가능 = Fast-forward

## 병합하기 2

- 헤드 브랜치에 추가적인 커밋이 생기는 경우,
- 진짜 병합이 필요해 진다.
- 충돌이 날 수 있다.

## Pull

- 혼자 작업할때 pull이 필요한 경우 : 회사컴퓨터로 작업한 뒤 push한 후 집 컴퓨터에서 가져올 때.

## 충돌 해결
- 1 : 직접 그 코드에서 원하는 대로 수정.
- 2 : main과 branch중 main쪽을 고르고 싶을 경우, 충돌파일 우클릭 -> 충돌 해결 -> 내 것으로 충돌 해결 클릭.
- 3 : branch쪽 고르고 싶을 경우, 똑같이,,,  저장소 것을 사용하여 해결 클릭.

## 커밋 되돌리기

### reset

- 쉽지만 커밋이 날아간다.
- 강제 푸시가 필요하다. (오늘 내가 겪은 오류. 로컬이 더 최신인데 push 할려고 할 때.)
- 다른 방법 : 병합(내것으로 충돌 해결 클릭) 후 푸쉬.
- 자칫 되돌릴수 없기때문에, 비추하는 방법이다. 밑의 branch가 더 안전하다.

### 브랜치를 만들어서 되돌리기

- reset과는 달리, 커밋이 사라지지 않는다. -> 안전. 추천. 기록이 남음.
- 유일한 단점 : 트리가 지저분해진다. (혼자서 일 할 때는 단점이라고 보기 힘듦)


### revert를 이용해서 되돌리기
 - 이전 커밋을 복사해서 새로운 커밋으로 생성. 익히기만 하면 깔끔 간편하다.
 - 단점 : 충돌이 나기 쉽다.
 - 2번, 3번, 여러번 되돌리기 : 커밋1 - 커밋2 - 커밋3 했을 경우, 커밋1로 가고싶다면,
    커밋3에서 되될리기 -> 커밋2에서 되될리기 클릭.


## 커밋 덮어쓰기

- 의미없는 커밋 -> 의미있는 커밋 으로 커밋 할 때, 굳이 의미없는 커밋 남기고 싶지 않다면
   의미있는 커밋 커밋할 때 커밋 옵션 -> 마지막 커밋 정정 선택.


## 스태시

- 아직 이해가 안 된다. 다음에 또 보자.

##기타 주의 사항

- 주석을 남기지 말자(?)
- 좋은 커밋의 단위 : 자주 하자.
- (중요) 커밋 메시지를 잘 쓰자! 깃허브를 프로필로 제출했다면, 커밋 메시지를 본다!
