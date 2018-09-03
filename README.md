## 강의노트
[![강의노트 바로가기](https://upload.wikimedia.org/wikipedia/commons/4/4a/Aviso_%22categor%C3%ADzame%22_%28espa%C3%B1ol%29.svg)](https://github.com/kyagrd/PL2018Fall/wiki)

## 수업 내용 개요
기본개념, 함수형 프로그래밍 기초 (Haskell), 정규식과 유한오토마타,
람다계산법, normalization, evaluation, call-by-value, call-by-name, call-by-need
장난감 함수형 언어 인터프리터, 타입 검사, polymorphism, overloading
타입 유추, 일치화(unification), 논리형 프로그래밍(logic programming)

## 수업에 사용할 책
 * [새로 보는 프로그래밍 언어](http://www.acornpub.co.kr/book/programming-language)
 
     이 책은 Programming Language Pragmatics, 2nd edition을 우리말로 옮긴 번역서이다.
     하지만 이후로 개정판이 한 번 더 나와 원서 최신판
     [Programming Language Pragmatics, 3rd edition](https://www.elsevier.com/books/programming-language-pragmatics/scott/978-0-12-374514-9)의 내용도 필요에 따라서는 수업에 활용할 수 있다.
     수업은 이 책의 내용을 순서대로 처음부터 끝까지 따라가는 것이 아니다.
     이 책은 비교적 최신의 프로그래밍 언어 관련 지식을 폭넓지만 이론과도 연계하여 소개하고 있어 프로그래밍 언어들의 특징과 차이점 및 공통점을 파악하기 좋게 되어 있어 수업에서 다루지 않는 내용도 스스로 읽어볼 것을 권한다.
     수업의 주요 내용은 함수형 프로그래밍 언어(functional programming language)와 논리형 프로그래밍 언어(logic programming language)와 관련된 이론과 활용을 소개하는 데 맞추어져 있다.
     
 * [Programming in Haskell, 2nd edition](http://www.cs.nott.ac.uk/~pszgmh/pih.html)
 
     정말 잘 쓰여진 책이며 두 파트로 나눠져 있는데 첫 파트는 처음 프로그래밍을 배우는 사람들을 대상으로 (책을 지은 교수님이 재직하시는 영국의 대학교 컴퓨터과학과 1학년 학생 대상으로) 하고 있어 하스켈의 기능을 엄선된 예제와 함께 찾아보며 스스로 학습하기에 좋다.
     이 강의의 주목적은 하스켈에 능숙하게 되는 것이 아니기 때문에 강의에 필요한 최소한만 설명하고 넘어가게 될 것이므로 나머지 의문나는 부분을 스스로 찾아보며 공부할 수 있는 참고서로 사용할 목적으로 선정한 부교재이다.
     학구적이면서도 간결한 영어 문장으로 쓰여져 있어서 읽어보면 영어공부 특히 기술적/학문적 글쓰기를 할 때 어떻게 문단을 전개해야 하는지도 공부가 되어서 꼭 원서도 구비해서 참고하며 공부하면 좋다.
     이 책의 예제중에 몇가지를 그대로 혹은 약간 변형해서 수업에서도 일부 활용할 예정이다.

## 수업에 사용할 SW

 * [IHaskell](https://github.com/gibiansky/IHaskell) - [Haskell](http://haskell.org) 프로그래밍 언어를 지원하나는 [Jupyter](http://jupyter.org) 커널
   - Docker for Toolbox를 이용한 IHaskell 설치 방법 [안내 영상](https://youtu.be/rvaXWrN6tJY)
       - 참고로 더 최신 버전 소프트웨어로 구성된 도커 이미지가 만들어진 관계로
         영상에 화면에 나오는 명령어 대신 아래와 같은 명령어를 사용하도록 한다.
         ```
         docker run -it -v "`pwd`":/home/jovyan/ihaskell/notebooks -p 80:8888 kyagrd/ihaskell
         ```
   - 최신 버전의 Mac OS X 및 Windows 10 Professional 에서 메모리 8GB이상을 갖춘 환경에서는
     Docker for Toolbox 대신 더 최신 버전의 도커 소프트웨어인 Docker for Mac이나 Docker for Windows를 사용해도 된다.
   - Linux를 사용하는 경우라면 설치가 더 간단하다. 배포판 docker 패키지로 docker 소프트웨어 설치 후 명령어를 실행하면 된다. 
 * 후반부에 Logic Programming을 소개할 때 사용할 소프트웨어는 추후 공지할 예정
