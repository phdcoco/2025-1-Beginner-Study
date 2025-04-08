# Week 3

## 커밋 수정

git commit —amend를 사용한다.

방금 한 **마지막 커밋**을 다시 수정하고 싶을 때 쓰는 명령어이다.

완전히 새로운 commit으로 대체되며, commit id가 바뀐다. 이때 vim편집기가 실행됨.

git commit —amend **-m** “메시지” 처럼 -m을 이용하면 vim 진입 없이 수정이 가능하다.

git commit —amend —no-edit 은 파일만 추가하고나 삭제할 때 커밋 변경 없이 수정 가능하다.

## 커밋 제거

git reset —option commitID 꼴로 사용한다.

- reset —soft
    - 최근 커밋만 취소한다.
    - 파일들은 그대로 스테이징 상태가 된다. (Staging Area)
    - 주로 커밋 메시지를 바꿀 때 씀
- reset —mixed
    - 커밋을 취소한다.
    - 파일도 스테이징에서 내려진다. (Working Directory)
- reset —hard
    - 커밋을 취소한다.
    - 변경 사항을 모두 제거하고 이전 커밋으로 돌아간다.

## 커밋 변경 취소

이전에 했던 작업을 취소하는 새로운 행동.

A — B — C 에서 C가 실수라면 A — B — C — D가 됨.

이때 D는 C의 작업을 취소하는 커밋이 포함되어 있고, B와 비슷하지만 해시와 커밋 내용은 다름!!

→ 기록을 남기고 추적이 가능, reset보다 안정적이다.

revert —no-edit : 편집기 진입 없이 바로 revert 가능

revert —no-commit : 직접 커밋하지 않고, revert 내용을 Staging Area에 올림.