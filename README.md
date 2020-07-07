### 내 개발 일지

### 컴퓨터 네트워크

*  Layer 0 관련 개념
   *  토폴로지: 네트워크가 구성되는 위상
   *  라우팅 루프: 패킷이 회로에서 무한 반복 돈다
   *  트리 네트워크: 컴퓨터 네트워크가 주로 구성되는 방식, 위상
   *  트레픽 엔지니어링: 패킷 충동을 방지하기 위한 기술
   *  패킷: 고정 길이 이다. 왜냐하면 파일 사이즈 만큼 패킷을 지정한다면 팻킷이 누락되거나 회로를 다른 패킷과 공유하기 어렵기 때문이다.
   *  bandwidth delay, propagation delay, store and forward delay queuing delay은 ethernet 혹은 WIFI의 속도 혹은 성능을 측정 개념 용어이다.
*  용어 정리
   *  LAN(Local Area Network): 네트워크의 물리적 개념이고 컴퓨터간 상호 연결하는 네트워크이다.
   *  datagram forwading: NAT, 방화벽, sliding_windows, 패킷 충돌, packet based switching, routing 따위와 연관 되는 기술이다.
   *  data rate: kbps, mbps, 데이터 전송 성능이다. Throughput bandwith 개념과 연결되는 용어이다.
   *  TTL(Time To Live): 패킷이 라우터를 지날떄마다 1씩 감소한다. 주로 64로 설정되어 있으며 라우팅 루프 현상을 방지한다.
      





### Linux

*  ubuntu
   *  about Ubuntu
      *  유분투는 데비안 구조와 인프라를 기반으로 한다. 6개월마다 업데이트(LTS:release every two years) 되며 데스크탑 서버, IOT 와 로봇 에디션이 있다.
      *  [공식 웹사이트](Ubuntu.com)
      *  [데스트탑 버젼 다운로드](https://ubuntu.com/download/desktop/thank-you?version=20.04&architecture=amd64)
   *  Ubuntu 권한 설정 명령어들
      *  리눅스 시스템에서 보안은 먼저 시스템에 대한 사용자 계정 및 서비스 엑세스를 제한하는 것이다. 그런 후, 보안은 주위가 설정 한대로 방어가 되었다는 것을 의미한다.
      *  사용자 및 그룹 작동하기
         *  su 혹은 sudo로 root 사용자를 사용한다
      *  root 로그인을 비활성화 시켜 보안을 강화한다.
      *  `useradd` 사용자 추가
      *  `userdel` 사용자 삭제
      *  `groupadd` 구룹 추가
   *  내장된 방화벽 추축하기
   *  시스템 로그 구성하기
   *  고급 보안 기능
      * 보안 강화 리눅스(SELinux)
   
   *  그 외 [Linux man pages](https://linux.die.net/man/) 참고
       
*  centOs
   *  about CentOs
      *  레드헷 제휴로 개발한 커뮤터 운영체제이다. 무료 기업용 컴퓨팅 플랫폼을 제공할 목적으로 만들어진 리눅스계 운영 체제 가운데 하나이다.
      *  레드헷 엔터프라이즈 리눅스의 소스 코드를 그대로 가져와 빌드해 내놓으며 이과정에서 이루어지는 변형은 레드헷의 상표가 잘리고 그자리에 CentOS의 상표가 붙는(상표권 분쟁을 피하기 위해)
      정도뿐이다.
      *  [공식 웹사이트](https://www.centos.org/)
      *  [CentOS 다운로드](https://www.centos.org/download/)
      
*  데비안과 레드헷 엩터프라이즈 리눅스 또는 페도라 세스템의 차이점
   *  리눅스 설치 과정은 복잡하다. 우분트는 이러한 설치과정을 보편적인 사용자가 수용할 수 있는 부분만 제외하고 나머지는 자동화해 놓음으로써 몇 번을 클릭만으로 설치가 가능하다.
      레드헷 시스템의 경우에는 사용자에게 워크스테이션 도는 서버, 설치할 개별 패키지 선택, 그리고 설정 옵션등 많은 설치 옵션을 제공한다.
   *  소프트웨어 관리 툴
      *  데비안: APT(Advanced Package Tool): 설치, 사제, 질의 업데이트 기능 사용
      *  레드헷: RPM
   *  GUI 툴이나 드롭다운 메뉴에서의 이들의 위치 등은 완전히 다르다.
      

### Node Js
  *  설치 과정
     *  [node js 다운로드](https://nodejs.org/ko/download/)
      ![노드다운로em](https://user-images.githubusercontent.com/12722674/86677033-2f25e100-c036-11ea-9d83-064e700a54f0.png)
      
     *  설치 확인 명령어: `node -v`
     
     ![2020-07-07 09_44_15-명령 프롬프트](https://user-images.githubusercontent.com/12722674/86677341-790ec700-c036-11ea-806d-cc781812e8fd.png)
     
     현제 필자의 컴퓨터에는 12.13.0 버젼이 설치되어있다.


### AWS

### RDBMS

### Node Js

### PostMan

### MySql Workbench

### github

### Anaconda

### Juypeter noteBook

### Docker

### Slack

### Trello
