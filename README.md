<div align="center">
    <h1>짧은 Git 가이드</h1>
    <h6>길게 설명하지 않아 숙련자들이 간단하게 보기 좋은 가이드</h6>
</div>

## 최초설정
깃 사용자 이름 설정
```git
git config --gloabl user.name <이름>
```

깃 사용자 이메일 설정
```git
git config --global user.email <이메일>
```

## 저장소 생성과 커밋
저장소 복제 ( 원격 경로 입력시 remote origin 자동 추가 )
```git
git clone <로컬 및 원격 경로>
```

깃 레파지토리 초기화
```git
git init
```

깃 상태 확인
```git
git status
```

커밋 대기열에 특정 파일 추가
```git
git add <파일명>
```

커밋 ( -m 옵션 없으면 vim으로 메세지 작성 )
```git
git commit -m <메세지>
```

## 브랜치
브랜치 확인
```git
git branch
```

브랜치 생성
```git
git branch <브랜치명>
```

브랜치 삭제
```git
git branch -d <브랜치명>
```

현재 사용중인 브랜치 변경
```git
git checkout <브랜치명>
```

현재의 브랜치를 특정 브랜치와 합치기
```git
git merge <특정 브랜치명>
```

## 브랜치 병합 충돌관리


## 원격 저장소
원격 저장소 확인
```git
git remote
```

원격 저장소 관리 추가
```git
git remote add <관리명> <원격 저장소 주소>
```

원격 저장소 관리 삭제
```git
git remote remove <관리명>
```

원격 저장소 가져와서 로컬과 병합
```git
git pull <관리명> <해당 브랜치>
```

원격 저장소와 전혀 관련 기록이 없는 로컬과 병합
```git
git pull <관리명> <해당 브랜치> --allow-unrelated-histories
```

원격 저장소에 변경 사항 올리기 ( -u 옵션 넣으면 추후에는 git push만으로 업로드 가능 )
```git
git push <관리명> <해당 브랜치>
```

원격 저장소에 강제적으로 올리기
```git
git push <관리명> +<해당 브랜치>
```

원격 저장소에 브랜치 삭제하기
```git
git push <관리명> -d <해당 브랜치>
```