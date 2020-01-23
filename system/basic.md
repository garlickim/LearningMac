## Homebrew
Max Os에서 제공하지 않는 패키지들을 설치하고 관리할 수 있는 패키지 관리자
<br>

터미널에서 하기 명령어 실행  
~~~linux
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
~~~
  
  
참고 : https://brew.sh/index_ko


<br><br><br>

## jenv
여러 버전의 Java를 사용하는 경우, Java 버전을 관리해주는 패키지  
내가 사용한 명령어는 bash shell을 사용하는 경우 
<br>

> jenv 설치
~~~linux
brew install jenv
~~~

<br>

> bash shell에 추가
~~~linux
echo 'export PATH="$HOME/.jenv/bin:$PATH"' >> ~/.bash_profile  
echo 'eval "$(jenv init -)"' >> ~/.bash_profile
source ~/.bash_profile
~~~

<br>

> jenv에 내가 설치한 2개의 JDK을 추가
~~~linux
jenv add /Library/Java/JavaVirtualMachines/adoptopenjdk-11.jdk/Contents/Home
jenv add /Library/Java/JavaVirtualMachines/jdk1.8.0_121.jdk/Contents/Home
jenv add /Library/Java/JavaVirtualMachines/jdk1.8.0_111.jdk/Contents/Home
~~~


참고 : https://www.jenv.be/  
https://jogeum.net/15
