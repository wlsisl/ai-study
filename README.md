# ai-study
github, R언어, 파이썬, 빅데이터 공부

<H2>1.GitHub 알아보기</H2>
<h4>공부하기에 앞서 GitHub에 대해서 알고가자</h4>
<h4>github란?</h4>
소프트웨어를 개발하는 과정에서 버전을 컨트롤하는 것을 웹상에서 도와주는 사이트이다. 
[출처] [깃허브] github 사용법 초보자|작성자 메카닉

다른 사람들과 프로젝트를 함께 할 수 있도록 도와준다. control과 collabotration을 돕는다.
팀원들이 함께 수정할 수 있고 변경이력을 보고 수정했던 때로 돌아가서 확인할 수 있다.
기본적으로 repository, branch, commit, push 등을 익힐 필요가 있다.

* repository
<br>project를 저장하는 저장소를 말한다. 이때 readme를 설정하면 마크다운 문법을 활용할 수 있다.</br>

* branch
<br>메인을 복사해서 새로운 프로젝트를 만들어 테스트해보는 곳이다.</br>

* commit
<br>깃허브에 저장된 변경사항이다. commit을 할 때마다 gutbub에 변경시점이 기록되고 다른 사람들이 확인 가능하다.</br>

* push
<br>저장된 commit을 원격저장소에 업로드 하는 것이다.</br>

* pull request
<br>다른 사람들의 수정사항을 보고 적용 유무를 판단하는 단계이다. 최근 작업 내역을 볼 수 있다.</br>
commit 확인->create pull request클릭->open a pull request->어떤 변화 있었는지 입력하기

<hr></hr>
<h2>2.R언어</h2>
**r을 왜 사용하는가?**

1. 재현가능성 - 이전에 했던 분석을 다시 재현할 수 있다.   
2. 자동화- 데이터가 변하거나 무엇인가 잘 못 되었을 경우 분석을 다시 신속하게 할 수 있다.   
3. 소통- 프로그래밍 코드는 텍스트이다. 세계적인 기업들이 R을 사용하므로 여러 사람들에게 도움 받을 수 있다.

**R의 특징은?**

<h>통계데이터수정과 분석에 주로 사용되는 언어이다. 시각화에 월등하며 무료프로그램이다.
일반적인 프로그래밍이 가능하고 새로운 함수를 생성할 수 있다.
오픈소스 소프트웨어임으로 사용자들이 수많은 함수를 공유하고 있다. R의 응용영역은 꾸준히 확장되는데, 통계처리를 위한 목적으로 개발되었지만 현재 머신러닝/딥러닝, 데이터마이닝 자연어처리 등 다양한 분야로 응용범위를 넓혀가고 있다.
데이터분석 또는 시각화가 목적이라면 R언어를, 웹 애플리케이션과 연동할 목적이라면 python을 사용한다. R은 인터프리터언어이다. R은 입력한 코드를 컴파일 과정 없이 직접 실행시킴으로써 과정을 편하고 간결하게 만들어준다.</h>

**R을 활용한 데이터 시각화 예**

>  나이팅게일 차트, 파이차트, 상관행렬 히트맵   
   1에 가까울수록 비례, -1에 가까울 수록 반비례, 0에 가까울 수록 관련없다.

**R program을 설치하기**

google에 cran(The Comprehensive R Archive Network)검색 -> Download R for 운영체제 -> base링크->download누르기

**창**

 r명령어 입력 -> 콘솔 창
 r그래프 -> r그래픽창
 r스크립트파일 -> r 편집기창

*RGui 창 내에서만 생성되도록 할 때는 MDI모드
*개별 창들이 독립적으로 움직이게 하고 싶으면 SDI모드   
*모드는 이후에 Rconsole파일에서 변경 가능하다.#으로 막을 수 있다.   

Rconsole창에서 명령어를 입력 but Rstudio를 더 많이 이용함. Rconsle은 괄호 사용이 많아지기 때문에.
여러개 명령어를 입력하고 싶다면 R편집기 창을 이용하기

**Rstudio알아보기**

source창 (색깔 구분, 필요한 괄호 만들어줌) = R편집기 창
<hr></hr>

<h2>컴퓨터 구조</h2>
*기계어(Machine Language): 0과 1로 표현된 언어*

*어셈블리어(Assembly Language):기계어와 일대일 대응하는 언어*

*고급언어(High Level Language):인간 입장에서 컴퓨터에게 명령을 내릴 수 있도록 구성된 언어*

<h4>Hardware</h4>
##cpu와 memory, i/o device가 연결되어있다.
CPU(Central Processing Unit): 산술연산/관계연산/논리연산
연산 자체는 담당하지만 기억기능이 없다.
   ALU(Arithmetic Logical Unit):연산
  
   CU(Control Unit):제어   
   
   Register:임시 기억 장소   

Memory:프로그램(명령의 집합)이나 데이터(값)를 기억  

   RAM(Random Access Memory):주로 사용하는 메모리, 전원이 연결된 상태에서만 저장, 읽기/쓰기 모두 가능
   
   ROM(Read Only Memory):기억기능밖에 없어서 RAM에 복사되어 사용된다. 속도가 느림.
   
I/O(input/output)Device:입/출력 장치
   input Deice(입력장치): 키보드, 마우스, 마이크, 카메라, **입력내용은 Memory에 저장된다.**
   
   Output Device(출력 장치):모니터, 스피커, 출력내용은 Memory에 있는 내용을 출력한다.(그러니까 컴퓨터 하드웨어 장치를 동작하는 것은 명령으로 제어를 할텐데 명령을 내리기 위해서 어떤 장치가 작동되게 해야할까? 
   
   2nd Memory(보조 기억 장치):HDD, SSD, Memory에 보관되었던 프로그램이나 데이터를 보관하는 목적의 저장 장치. 즉 Memory는 전원이 연결된 상태에서만 저장해주기 때문에 이를 대신해준다.
   
<h4>Software</h4>
컴퓨터 시스템의 기계장치를 운영하는 프로그램

   * System Software: 우리는 cpu, memory, i/o device에 명령을 내릴 수 있어야한다. 즉 H/W를 제어하고 Application Software를 동작할 수 있는 환경을 제공하는 프로그램   
   O/S(Operation System):Windows/Linux/Mac OS
   
   * Library:Application Software가 사용하는 함수 집합
   
   * **Application Software: 일반 사용자를 위한 프로그램, End-user를 위한 프로그램

+컴퓨터 네트워크(computer network):컴퓨터간 통신(데이터공유, 프로그램 공유)을 수행할 수 있도록 연결

+LAN(local area network):좁은 지역의 컴퓨터를 연결한 network

+WAN(wide area network):넓은 지역의 컴퓨터를 연결한 network

+internet:전세계 컴퓨터를 연결한 network

+프로토콜 (protocol):네트워크에 연결된 컴퓨터간 통신을 하기 위한 규칙

+TCP/IP:internet에서 사용하는 protocol

+WWW(world wide web): internet에서 제공하는 서비스 형태

+HTTP: wep에서 사용하는 protocol

+HTML: web에서 제공되는 서비스를 구현할 때 사용하는 프로그램 언어

+server computer: 요청에 대한 응답을 수행하는 컴퓨터
   - server program: Server computer 에서 요청에 대한 응답 처리를 수행하는 프로그램
+client computer: 요청을 하는 컴퓨터
   - Client program: Server computer 에게 요청하는 처리를 수행하는 프로그램
   
+cloud service: server computer에 있는 공간(물리적인 공간 또ㅗ는 서비스를 제공하는 프로그램)을 사용자에게 대여해주는 서비스, 반드시 internet에 연결된 상태이어야한다. web browser를 사용하여 cloud service를 이용한다.

<hr></hr>
<H2>Python</H2>
본 과정은 머신러닝에 필요한 파이썬 프로그래밍 부터 데이터 분석 및 시각화 다양한 알고리즘 등을 학습한다.

<h4>1.파이썬 개념과 특징</h4>
개념: 컴퓨터 시스템에게 명령을 내리기 위한 용도로 사용하는 프로그램언어

<h4>2.파이썬 개발과정</h4>
먼저 파이썬 개발과정부터 살펴본다. 
