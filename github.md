# GitHub

## 기초 명령어

<br>

### 원격 저장소 복제

```
git clone <url>
```

<br>

### 원격 저장소 정보 확인

```
git remote -v
```

<br>

### 원격 저장소 추가

일반적으로 원격 저장소명으로 origin 사용

```
git remote add <원격저장소> <url>
```

<br>

### 원격 저장소 삭제

```
git remote rm <원격저장소>
```

<br>

### 원격 저장소에 push

```
git push <원격저장소> <브랜치>
```

<br>

### 원격 저장소로부터 pull

```
git pull <원격저장소> <브랜치>
```

<br>
<br>

## 브랜치 주요 명령어

<br>

### 브랜치 생성

```
git branch <브랜치>
```

<br>

### 브랜치 이동

```
git checkout <브랜치>
```

<br>

### 브랜치 생성 및 이동

```
git checkout -b <브랜치>
```

<br>

### 브랜치 목록

```
git branch
```

<br>

### 브랜치 삭제

```
git branch -d <브랜치>
```

<br>

### 브랜치에서 작업한 이력 합치기

master 브랜치로 이동 후 merge

```
git merge <브랜치명>
```
