# Tips for IntelliJ
인텔리제이의 강력한 활용을 위한 Mac OS 기준의 팁 정리

## Toolbox
- Jetbrains 제품을 통합 관리해주는 소프트웨어
- IntelliJ Setting -> Maximum heap size 설정 (메모리가 16GB이라면 4GB로)

## 프로젝트 생성
- Dracula 테마 선택
- Mac OS X 10.5+ Keymap 선택
- GroupId: 전체 프로젝트 (ex. 스프링 프로젝트)
- ArtifactId: 그룹의 하위 모듈 (ex. 스프링 시큐리티, 스프링 MVC)

## 프로젝트 Shortcut
- Shift + Shift: All, Classes, Files, Symbols, Actions, Git 검색
- Cmd + Shfit + O : 파일 검색
- Cmd + Opt + O : 심볼(메소드) 검색
- Cmd + Shfit + A : Action 겸색

## 파일 Shortcut
- 생성 및 실행
  - Cmd + N: 현재 환경에서 만들 수 있는 New 리스트를 보여줌
  - psvm: public static void main 을 자동으로 만듦
  - sout: System.out.println 을 자동으로 만듦
  - iter: index가 없는 iterable 객체를 순회하는 반복문을 자동으로 만듦
  - itar: index가 있는 리스트 형태 객체를 순회하는 반복문을 자동으로 만듦
  - psfs : public static final String 을 자동으로 만듦
  - psfi : public static final int 을 자동으로 만듦
  - Ctrl + Shift + R: 현재 포커스를 실행
  - Ctrl + R: 오른쪽 상단에 표기되는 방금 이전 포커스를 실행
- 라인 수정하기
  - Cmd + D: 현재 라인 아래로 복제
  - Cmd + backspace: 현재 라인 삭제
  - Ctrl + Shift + Z: 문자열 사이의 + 연산을 문자열 하나로 합쳐줌
  - Opt + Shift + 위아래 방향키: 구문에 관계 없이 라인 강제 이동
  - Cmd + Shift + 위애래 방향키: 구문 안에서 라인 이동
  - Cmd + Opt + Shift + 좌우 방향키: html이나 XML 같은 엘리먼트 언어에서 앨리먼트 단위 좌우 이동
  - Cmd + OPt + L: 프로젝트 포맷 정의에 따라 자동으로 포맷 지정
  - Cmd + Z: undo
  - Cmd + Shift + Z: undo의 undo
  - Cmd + C: 복사
  - Cmd + V: 붙여 넣기
- 코드 즉시보기
  - Cmd + P: 함수 호출에 필요한 인자값을 피킹
  - Opt + Space: 함수 정의부를 피킹
  - F1: 자바 doc 피킹
  - Cmd + B: 호출부에선 선언으로 이동, 선언부에서는 호출부로 이동
- 포커스 에디터
  - Ctrl + A: 해당 라인 맨 앞으로 이동
  - Ctrl + E: 해당 라인 맨 뒤로 이동
  - Opt + 좌우 방향키: 단어별 이동
  - Opt + Shift + 좌우 방향키: 단어별 선택 이동
  - Fn + 위아래 방향키: 한 페이지씩 이동
- 포커스 특수키
  - Opt + 위 방향키: 포커스 위치의 어구 단위 점차적으로 선택
  - Opt + 아래 방향키: 포커스 위치의 어구 단위 점차적으로 선택 해제
  - Opt + Opt + 위 아래 방향키: 멀티 포커스
  - F2: 오류가 있는 곳으로 포커스 이동
- 검색 텍스트
  - Cmd + F: 현재 파일에서 검색
  - Cmd + Shift + F: 파일과 파일 내용을 전체 프로젝트에서 검색
  - Cmd + R: 텍스트 교체
  - Cmd + E: 최근에 연 파일 리스트 검색
  - Cmd + Shift : 최근에 수정한 파일 리스트 검색
- 자동완성
  - Cmd + N: Getter/Setter/ 생성자 자동 완성
  - Ctrl + I: 구현해야하는 추상 메소드 자동 완성
- Live Template
  - Live Template 설정 창에서 다양한 축약어들을 커스터마이징하여 설정할 수 있음
- Extract
  - Opt + Cmd + V: 선택 곳을 변수로 추출하기
  - Opt + Cmd + P: 선택 곳을 파라미터로 추출하기
  - Opt + Cmd + M: 선택 곳을 메소드로 추출하기
  - F6: 선택한 이너 클래스 추출하기
- 리팩토링
  - Shift + F6: 변수/메소드의 이름 일괄 변경
  - Cmd + Shift + F6: 타입 일관 변경
  - Ctrl + Opt + O: 사용하지 않는 Import 문 정리
  - Cmd + Opt + L: 프로젝트 포맷 기준에 맞춰 코드 자동 포맷 정렬
- 터미널
  - Opt + F12: IDE 내장 터미널을 열어줌
## 디버깅
- Ctrl + Shift + D: 현재 포커스를 디버그 모드로 실행
- Ctrl + D: 오른쪽 상단에 표기되는 방금 이전 포커스를 디버그 모드로 실행
- BreakPoint
  - BreakPoint는 코드와 라인 넘버 사이에 마우스로 클릭을 하면 설정 가능
  - Coditional BreakPoint는 BreakPoint를 우클릭으로 누르고 조건에 자바 코드를 추가해서 설정 가능
  - Opt + Cmd + R: Resume, 다음 BreakPoint로 이동
  - F8: Step Over, 현재 BreakPoint의 다음 한줄로 이동
  - F7: Step Into, 현재 BreakPoint의 코드 안으로 들어가서 이동
  - Shfit + F8: Step Out, Step Into로 안으로 포커스가 들어 왔을 때 다시 밖으로 이동
  - Opt + F8: Evaluate Expression, 현재 BreakPoint 시점부터 코드를 단발성으로 실행해볼 수 있음
  - Watch는 BreakPoint가 걸린 이후에 안경 모양 아이콘을 통해서 설정할 수 있고 input 창에 관찰할 변수 이름을 설정해서 브레이크 이후에도 실시간 값의 변화를 알 수 있음 

## Git

## 플러그인
- .ignore: .gitignore에 자동 완성 및 기본 ignore 파일을 제공하는 플러그인
- BashSupport: 쉘 코딩에서 자동 완성 및 문법 체크에 도움을 주는 플러그인
- CheckStyle-IDEA: 체크 스타일 파일이 있을 때 설정할 수 있게 해주는 플러그인
- 깃 툴박스: 깃 활용할 때 도움이 되는 플러그인
