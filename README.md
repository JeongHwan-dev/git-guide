# :octocat: 깃 가이드(Git Guide)

## 1. 개요(Outline)

**Git(깃)** 은 컴퓨터 파일의 변경사항을 추적하고 여러 사용자들 간에 해당 파일 작업을 조율하기 위한 대표적인 `버전 관리 시스템(VCS)`입니다.

<br />

## 2. 깃 명령어(Git Commands)

### 깃 초기화

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
$ git config --global user.name 'JeongHwan-dev'
```

#### 이메일 설정

```bash
$ git config --global user.email 'jeonghwan.dev@gmail.com'
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

### 스테이지에 올라온 파일 커밋

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
$ git push origin master
```
