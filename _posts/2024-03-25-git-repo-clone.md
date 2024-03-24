---
title: "git repository 복사, 깃 레포지토리 복사"
categories:
  - Blog
tags:
  - git
  - 테스트
---

깃랩 <> 깃허브로 이관하거나

새로운 레포지토리로 깃 전체를 이관 혹은 해당 브랜치만 이관할때 사용하는 명령어    

> 깃 저장소 복사

```bash
# 깃 전체 복사 (전체 브랜치 포함)
$ git clone --mirror { git 주소 }

# 특정 브랜치만 참조하여 복사
$ git clone -b { 브랜치명 } --single-branch --mirror { git 주소 }
```

> 복사 후 깃 이관 작업 진행 

```bash
# 생성된 레포지토리 git폴더 내부로 이동
$ cd { 레포명.git }

# 이동한 git 폴더 내부에서 레포지토리 주소 지정
$ git remote set-url origin { 새로운 repository 주소 }

```

