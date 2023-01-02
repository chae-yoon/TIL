# Git

## 기초 명령어

<br>

### 로컬 저장소 생성

```
git init
```

<br>

### 특정 파일/폴더의 변경사항 추가

```
git add <파일명>
```

<br>

### 커밋 (버전 기록)

```
git commit -m '<커밋 메세지>'
```

<br>

### 상태확인

```
git status
```

Tracked: 이전부터 버전으로 관리되고 있는 파일

- Unmodified: git status에 나타나지 않음
- Modified: Changes not staged for commit
- Staged: Changes to be comitted

<br>
Untracked: 버전으로 관리된 적 없는 파일(보통 새로 파일을 만드는 경우)

<br>

### 버전확인

```
git log
```

[마크다운 문법 정리 →](./markdown.md)
<br>

[GitHub 기반 원격저장소 활용 →](./github.md)

<br>

[Python 기초 →](./python/basic.md)
