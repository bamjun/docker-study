### 우분투 컨테이너 생성하기
```bash
docker run -it --name my-new-ubuntu-container ubuntu
```

### 종료
```bash
docker stop [container]
```

### 재접속
```bash
docker start -ai [CONTAINER]
```



```bash
apt update
apt install -y python3 git curl git wget vim zsh
chsh -s $(which zsh)
```


### Oh My Zsh 설치
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### OhMyZsh 자동완성설치하기
### zsh-autosuggestions


```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```bash
vim ~/.zshrc
```

```
plugins=(git zsh-autosuggestions zsh-completions)
```

```bash
source ~/.zshrc
```

### zsh-completions
```bash
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-completions
```

```bash
vim ~/.zshrc
```

```
plugins=(git zsh-autosuggestions zsh-completions)
```

```bash
source ~/.zshrc
```


### Powerlevel10k 테마 적용하기
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
source ~/.zshrc
```

### p10k 재설정
```bash
p10k configure
```


### homebrew 설치
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### homebrew 등록
```bash
echo 'eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"' >> /root/.zshrc
eval "$(/home/linuxbrew/.linuxbrew/bin/brew shellenv)"
```



---
---

### Oh My Zsh가 설치된 후, ~/.zshrc 파일을 편집하여 테마와 플러그인을 설정할 수 있습니다:
### Zsh 테마 변경
```bash
nano ~/.zshrc
```
`
### Zsh 재시작
```bash
source ~/.zshrc
```

### 시스템 기본정보를 확인
```bash
uname -a
```

### 배포판 정보 확인
```bash
cat /etc/os-release
```

### OS 이름과 버전을 포함한 시스템 정보를 확인
```bash
hostnamectl
```


### 현재 사용중인 쉘의 경로 확인
```bash
echo $SHELL
```

### 현재 실행 중인 쉘 프로그램의 이름을 출력
```bash
echo $0
```

### 현재 쉘의 프로세스 정보를 확인
```bash
ps -p $$
```

### 사용자의 기본 로그인 쉘을 확인
```bash
cat /etc/passwd | grep $USER
```

