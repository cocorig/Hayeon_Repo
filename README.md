# Hayeon_Repo
멋사 FES 7기 협업 실습용 레퍼지토리입니다. : )

## 목차
1. 깃허브 레파지토리 준비하기
2. 깃허브 프로젝트
3. 깃허브 이슈
4. 깃허브 이슈 제대로 사용하기
5. 깃허브 특강
6. 
## 체크리스트
- [x] 테스트 저장소 생성


## 깃허브 특강 정리

- git init : 깃허브에서 관리하는 컴퓨터에서 .git 파일이 만들어진다.   ->  깃허브에 git init이 만들어진다.
- git clone 레포지토리 주소 (원격 저장소에서 가져오기)
- git 은 실제 도구 코드관리,파일관리,코드관리(버전 관리 시스템) -> github는 실제 저장소 ,GitHub는  git을 사용자가 편리하게 사용할 수 있는 웹 서비스

내 컴퓨터 (로컬 저장소) 깃에 있는거 (원격 저장소)

- git add <추가할 경로> : 내 변경사항을 로컬에 있는 깃에다 적용을 한 것.
- git commit 'm'
- git status -  내 git의 현재상태를 본다
- git diff - (이전 기록)commit을 기준으로 변경사항을 본다



파일의 상태에 따라 **Untracked 와 Tracked 로 분류됩니다.**

1) **Untracked**(관리 대상이 아님) : 파일 생성 후 한번도 `git add`하지 않은 상태를 말합니다.

2) **Tracked**(관리 대상임) : git이 관리하는 파일임을 의미합니다.

- `Unmodified` : 최근의 커밋과 비교했을 때 바뀐 내용이 없는 상태
- `Modified` : 최근 커밋과 비교했을 때 바뀐 내용이 있는 상태
- `Staged` : 파일이 수정되고 나서 스테이지 공간에 올라와 있는 상태이며, `git add` 후의 상태

<img width="242" alt="" src="https://github.com/cocorig/Hayeon_Repo/assets/95855640/4182409f-f65c-4b9b-83d4-3bd081df16da">

💥 한번에 하는 작업단위로해서 commit 하기

- M    : 수정됨

- D    : 삭제됨 (git항목에서 표시)

- U    : 추적되지 않음. (git항목에서 표시)


기본적으로 1개의 브랜치는 존재합니다 !
그걸 기본브랜치라고 하구요
github에서 만든 레포의 main, git init을 통해만든 저장소의 master가 기본브랜치에 해당됩니다

git restore 
변경된 사항 -> modified된 변경사항을 복구시킨다
`restore`는 파일의 수정 내용 복원과 `add` 를 통해 스테이지에 올린 파일을 빼낼 때 사용합니다.

js의 모든 파일을 복구시킬 수도 있다.
git restore *.js

 -  restore 명령어를 이용하여 빼기

 - git restore --staged README.md


 - 특정 브랜치를 삭제하는 명령어 입니다.
 현재 main인 브랜치에 있다면 삭제되자않는다.
 - git branch -D <삭제할 브랜치명>