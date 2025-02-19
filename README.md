# CS-Study

## 참여 인원
| 권기범 | 김민수 | 성준영 |
| ---- | ---- | ---- |
| <img src="https://avatars.githubusercontent.com/u/111178301?v=4" width="230" height="230"> | <img src="https://avatars.githubusercontent.com/u/113896182?v=4"> | <img src="https://avatars.githubusercontent.com/u/103016359?v=4" width="230" height="230"> |

## 규칙, 일정
스터디의 자세한 규칙과 일정은 노션에 게재해두었다. <br>
<img src="https://img.icons8.com/?size=100&id=F6H2fsqXKBwH&format=png&color=000000" width="16" height="16"> [CS Study](https://wonderful-snowshoe-310.notion.site/CS-19dbd088fb1780be8198fe79fed9aca1)


## 파일명 
마크다운 파일은 [대목차][주제].확장자

<br>
<br>

## Pull Request 방법
- Fork
  ----
  본 리포지토리를 자신의 리포지토리로 fork 한다.
- clone, remote 설정
  ----
  fork로 생성한 본인 계정의 저장소에서 clone or download 버튼을 누르고 표시되는 url을 복사한다.
  
  자신의 컴퓨터에서 작업을 하기 위해서 Fork한 저장소를 로컬에 clone 한다.

  ```
  $ git clone https://github.com/Doritosch/CS-Study.git
  ```

  로컬 저장소에 원격 저장소를 추가한다. 위 작업과 동일하게 github 저장소에서 clone or download 메뉴를 통해서 확인한 url을 사용한다.
  - 원본 프로젝트 저장소 (직접 추가 필요)
  - fork한 로컬 프로젝트 (origin이라는 별명으로 기본으로 추가되어 있다. 따로 추가할 필요 없음)
  ```
  # 원본 프로젝트 저장소를 원격 저장소로 추가
  $ git remote add (별명) https://github.com/[원본계정]/CS-Study.git
  ```
  ```
  # 원격 저장소 설정 현황 확인방법
  $ git remote -v
  ```

- branch 생성
  ----
  자신의 로컬 컴퓨터에서 코드를 추가하는 작업은 branch를 만들어서 진행한다.
  ```
  # 자신의 이름의 branch를 생성한다.
  $ git checkout -b [이름]
  Switched to a new branch '[이름]'
  ```
- 자신이 공부한 내용 add, commit, push
  ----
  add, commit, push를 통해서 자신의 github repository (origin)에 수정사항을 반영한다.
  - **push 진행시에 branch 이름을 명시해주어야 한다.**
  ```
  # 자신이 만든 브랜치의 수정 내역을 origin 으로 푸시한다.
  $ git push origin [이름]
  ```
- Pull request 생성
  ----
  push 완료 후 본인 계정의 github 저장소에 들어오면 Compare & pull reqeust 버튼이 활성화 되어 있다. 

  해당 버튼을 선택하여 메시지를 작성하고 PR을 생성한다.
- Merge 이후 동기화 및 branch 삭제
  ----
  - 원본 저장소에 Merge가 완료되면 로컬 코드와 원본 저장소의 코드를 동기화 한다.
  - 작업하던 로컬의 branch를 삭제한다.
  ```
  # 코드 동기화
  $ git pull (remote 별명)
  # 브랜치 삭제
  $ git branch -d (브랜치 별명)
  ```
