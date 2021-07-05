# :octocat: 깃 가이드(Git Guide)

## 1. 개요(Outline)

**Git(깃)** 은 컴퓨터 파일의 변경사항을 추적하고  
여러 사용자들 간에 해당 파일 작업을 조율하기 위한  
대표적인 `버전 관리 시스템(VCS)`입니다.

<br />

## 2. 깃 명령어(Git Commands)

### 깃 초기화 (버전 관리 시작)

```bash
$ git init
```

### 깃 버전 확인

```bash
$ git --version
```

### 깃 설정

#### autocrlf 설정

- **Windows**

```bash
$ git config --global core.autocrlf true
```

- **Mac**

```bash
$ git config --global core.autocrlf input
```

#### 이름 설정

```bash
$ git config --global user.name 'YOUR_NAME'
```

#### 이메일 설정

```bash
$ git config --global user.email 'YOUR_EMAIL'
```

#### 깃 설정 확인

```bash
$ git config --global --list
```

### 깃 버전 관리 상태 확인

```bash
$ git status
```

### 파일 스테이징

- **특정 파일 스테이징**

```bash
$ git add 파일명
```

- **수정한 모든 파일 스테이징**

```bash
$ git add .
```

### 스테이지에 올라온 파일 커밋(버전 생성)

```bash
$ git commit -m 'message'
```

### 저장소에 저장된 버전 확인 및 커밋 기록 확인

```bash
$ git log
```

### 원격 저장소에 연결

```bash
$ git remote add origin 원격 저장소 주소
```

### 원격 저장소에 파일 올리기

```bash
$ git push -u origin master
```

### 브랜치 목록 조회

- **브랜치 확인(기본)**

```bash
$ git branch
```

- **브랜치 확인(원격 저장소 포함)**

```bash
$ git branch -a
```

### 새 브랜치 생성

```bash
$ git branch 새 브랜치 이름
```

### 브랜치 변경

```bash
$ git checkout 변경할 브랜치 이름
```

### 브랜치 생성과 동시에 변경

```bash
$ git checkout -b 새 브랜치 이름
```

### 원격 저장소 복제

```bash
$ git clone 원격 저장소 주소
```

### 버전 내역 되돌리기

- 한 커밋 이전으로 되돌리기

```bash
$ git reset --hard HEAD~1
```

- 두 커밋 이전으로 되돌리기

```bash
$ git reset --hard HEAD~2
```

- 다시 이전 커밋 상태로 되돌리기

```bash
$ git reset --hard ORIG_HEAD
```
