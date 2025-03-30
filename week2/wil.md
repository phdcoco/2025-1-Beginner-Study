### Week 2

## issue와 Branch, 그리고 Merge

# Issue

버그, 기능 제안, TODO, 질문 등 프로젝트와 관련된 어떤 것이든 자유롭게 기록하고 추적할 수 있는 기능

# Branch
1. 현재 브랜치 확인
- git branch로 내가 현재 어느 브랜치에서 작업하고 있는지 확인
- git branch -a 를 이용해 내가 지금까지 만든 브랜치가 무엇이 있는지 확인

2. 브랜치 생성 / 삭제

- git branch "브랜치 이름" 으로 생성
- git branch -D "브랜치 이름" 으로 삭제

3. 브랜치 이동

내가 작업하고 싶은 브랜치로 변경하기
- git checkout "브랜치 이름"

브랜치 생성 후 한번에 바로 이동하기
- git checkout -b "브랜치 이름"

4. 브랜치 활용하기

내가 작업한 파일 중 이 브랜치에다가 저장해야겠다! 할 내용들 모아두고
- git add 파일
- git commit -m "내용"
- git push origin 브랜치 이름

# Merge

Merge는 Github의 Pull requests에서 작업한다. compare에 벙합하려고 하는 브랜치를 선택한다.

1. Create a merge commit
- 기존 커밋 히스토리는 그대로 유지하고, 하나의 merge commit을 추가로 생성
- 즉, A, B, C의 커밋이 각각 main 브랜치로 병합함과 동시에 새로운 커밋 D를 만듦

2. Squash and Merge
- 하나의 커밋으로 main 브랜치로 병합

3. Rebase and Merge
- 브랜치의 커밋들을 main 브랜치 뒤에 이어붙이기만 하고, 병합 커밋 없이 병합한다.