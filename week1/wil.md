WEEK 1
=======
git으로 파일 관리하기
-------

##용어 정리
리포지토리(Repository) - 프로젝트가 저장되는 공간   
커밋(Commit) - 저장소에 저장하는 하나의 기록, 설명을 붙이고 저장하는 느낌   
브랜치(Branch) - 작업 공간을 나눔, 독립적으로 작업할 수 있는 하나의 가지   
푸시(Push) - 내 로컬 저장소에서 깃허브 저장소로 업로드   
풀(Pull) - 깃허브 저장소에서 내 로컬 저장소로 다운로드   

##기본 흐름
1. 깃허브에서 New repository 만든다.
2. 내 컴퓨터에서 작업 폴더 만들고 cd로 위치 설정 후 git init 한다.
3. git remote add origin https://github.com/phdcoco/프로젝트_이름.git 을 통해 깃허브 저장소 연결
4. 로컬 저장소에 만들었던 작업 폴더 안에서 파일을 만들고 작업한다.
5. 작업한 파일을 git add .를 통해 커밋할 준비를 하고.
6. git commit -m "이 파일에 대한 설명" 을 통해 저장소에 기록한다.
7. git branch -M main 으로 브랜치를 만든다.
8. git push -u origin main으로 커밋한 내용을 깃허브로 푸시한다. 이 다음부터는 git push만 해도 된다.   origin은 원격 저장소(기본값), main은 브랜치 이름이다.   
etc. git status는 변경된 파일 확인. git log는 커밋 기록을 확인한다.