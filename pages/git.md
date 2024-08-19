# Git 초심지를 위한 CheatSheet

> 로컬에 git repo clone

```bash
git clone [내려받을 저장소]
```

> 로컬에서 변경사항 모두 commit

```bash
git add .
git commit -m '커밋 메시지'
```

> 원격 저장소로 main브랜치로 변경사항 push

```bash
git push -u origin main
```

## 원본 원격 repo에서 업데이트 받아오기

내가 작업 중인 원격 저장소는 fork된 복제본이기 때문에 원본 저장소에서 데이터를 불러오려면 `git pull` 명령어로는 부족하다.

> 내 로컬 저장소에 원본 원격 저장소(upstream 별명으로) 추가

```bash 
git remote add upstream https://github.com/devPracticeCenter/kt_cloud_cicd_basic.git
```

> 원격 저장소 내용 동기화

```bash
git fetch upstream
```

> 원격 저장소 내용 내 로컬 main 브랜치에 병합

```bash
git rebase upstream/main
```

> 업데이트 된 로컬 main 브랜치를 내 원격 저장소(fork한 저장소) main브랜치로 덮어쓰기

```bash
git push --force -u origin main
```