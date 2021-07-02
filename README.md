# :octocat: 깃 가이드(Git Guide)

## 1. 개요(Outline)

**Git(깃)** 은 컴퓨터 파일의 변경사항을 추적하고 여러 사용자들 간에 해당 파일 작업을 조율하기 위한 대표적인 `버전 관리 시스템(VCS)`입니다.

<br />

## 2. 깃 명령어

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

**Windows**

```bash
$ git config --global core.autocrlf true
```

**Mac**

```bash
$ git config --global core.autocrlf input
```

#### 이름 설정

```bash
$ git config --global user.name 'JeongHwan-dev'
```

#### 이메일 설정

```bash
$ git config --global user.email 'jeonghwan.dev@gmail.com
```

#### 깃 설정 확인

```bash
$ git config --global --list
```

### 깃 버전 관리 상태 확인

```bash
$ git status
```
