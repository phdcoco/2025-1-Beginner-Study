### Week 1

## Git 코드 초기 설정 및 사용 정리

1. GitHub에서 리포지토리 생성
- 주소: `https://github.com/사용자 이름/리포지토리 이름

2. 로컬에서 Git 초기화 및 연결

cd ~/Desktop/2025-1-Beginner-Study
git init
git remote add origin https://github.com/phdcoco/2025-1-Beginner-Study.git

3. 첫 커밋 & 브랜치 설정

git add .
git commit -m "첫 커밋"
git branch -M main
git push -u origin main

4. 이후 반복 흐름 (파일 수정 또는 추가 후)

git add .
git commit -m "변경 내용 설명"
git push

5. ⚠️ 중간에 겪었던 에러와 해결 방법

- `error: remote origin already exists.`  
  → 이미 origin 연결되어 있음

- `main -> main (fetch first)`  
  → GitHub에 먼저 올라간 내용 있음

- `fatal: current branch has no upstream`  
  → `git push -u origin main`으로 해결

- `파일 수정했는데 git status에 안 나옴`  
  → VS Code 캐시 문제 → 껐다 켜기

## 다른 컴퓨터에서 내 리포지토리 가져와 저장하기

cd 저장하고 싶은 경로
git clone https://github.com/phdcoco/2025-1-Beginner-Study.git

## 상태 명령어

git status          # 현재 상태 확인
git log             # 커밋 기록 확인
git remote -v       # 원격 저장소 연결 상태 확인