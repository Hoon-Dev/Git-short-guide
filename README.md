<div align="center">
    <h1>짧은 Git 가이드</h1>
    <h6>길게 설명하지 않아 간단하게 보기 좋습니다.</h6>
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
레파지토리 깃 초기화
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
현재 레파지토리에 있는 브랜치 확인
```git
git branch
```

새로운 브랜치 생성
```git
git branch <브랜치명>
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