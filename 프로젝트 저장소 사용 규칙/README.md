# 프로젝트 협업 및 Github 이용 규칙 가이드

### 기본적인 설정들
**첫번째 설정**  
**git config --global user.name "github아이디"**  
**git config --global user.email "email"**  
만약 토큰 인증이 뜬다면 해당 token을 동일하게 config에 저장해서 해결합니다.
자세한 방법은 다음의 주소에 가서 참고해서 설정하기 바랍니다.  
[git token 로그인 방법](https://velog.io/@jini_eun/Github-2021%EB%85%84-8%EC%9B%94-13%EC%9D%BC%EB%B6%80%ED%84%B0-%ED%86%A0%ED%81%B0-%EC%9D%B8%EC%A6%9D-%EB%A1%9C%EA%B7%B8%EC%9D%B8-%EB%B3%80%ED%99%94).

**(부가/추가) 설정**  
**CLRLF 관련 설정**
기본적으로 프로젝트를 진행하는 모든 사용환경은 window이지만 프로젝트를 진행하다가 문제가 발생할 수 있으므로 해당 설정은 기본적으로 켜 적용합니다.  
**git config --global core.autocrlf true**  

### 저장소를 사용하기 위한 방법 및 규칙들

**git clone (github의 저장소 주소)**  
명령어를 통해 작업하는 저장소의 파일들을 자신의 컴퓨터에 복사하여 저장합니다.

### 두번째 (Branch 만들기)
이렇게 자신의 컴퓨터에 저장을 했다면 아래와 같이 자신이 작업을 진행할 새로운 branch를 만들어 해당 Branch에서 자신의 작업을 진행을 합니다.  
**git branch (branch name)**  
**git checkout (branch name)**  
**git switch (branch name)**  
위에 해당하는 모든 명령어는 Branch를 만드는 명령어입니다. 
자신이 원하는 명령어를 통해 사용하기 바랍니다.
만약 Banch를 만들고 바로 이동하기를 원한다면 다음의 명령을 사용해셔 진행을 합니다.

**git checkout -b (branch name)**  해당 branch를 만들고 바로 이동합니다.  
**git switch -C (branch name)**  해당 명령어도 같은 작업을 합니다.

### 세번째 (add 방법 및 commit 규칙)
#### git add *
기본적으로 해당 명령어를 사용하면 모든 파일들이 add가 되기는 하나 해당 기능은 되도록 사용을 자제하거나 사용하려고 한다면 ignore규칙을 정의해서 올라가면 안되는 파일들을 정의하고 사용하기 바랍니다.
**해당 규칙을 위반하면 안됩니다.**  

### git ignore규칙 정의 방법
### ex) echo *.doc > .gitignore

doc 파일에 대한 무시 설정
를 참고하거나 직접 ignore 파일에 들어가 해당 포맷을 추가합니다.
[gitigonre 관련 참고 사이트](https://velog.io/@psk84/.gitignore-%EC%A0%81%EC%9A%A9%ED%95%98%EA%B8%B0)


# 주의사항(merge)
프로젝트의 작업에 대한 merge는 
