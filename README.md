### Reason: Get to forget what I did for programming previously so record it in order to not reapeat same mistake other word repuce duplicate debugging
### 개발 기록
### Git 사용 시나리오 1
* Scenario one
  * 저자는 3개 커밋 로그를 남겼다
  * 4번째 커밋이 잘못됐다
  * 3번째 커밋으로 되돌리고 싶다(로컬저장소 혹은 working directory에도 3번째 커밋으로 동기화 시키고 싶다)
  * reset 혹은 revert을 할 지 햇갈린다
  * 3번째 커밋으로 돌아가는 revert를 시도 하였다.
  * 저자의 예상: 로컬저장소 혹은 working directory에도 3번째 커밋으로 동기화가 일어났다)
  * 실제 결과: to be continued....
* revert vs reset
   * reset은 Head를 변경시키고 revert는 Head를 최신상태로 유지하면 서 변경시킨다 continued....
   * https://velog.io/@njs04210/Git-reset%EA%B3%BC-revert-%EC%95%8C%EA%B3%A0-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0  <--참고하자
 ### Git 용어 정리
 * https://ordo.tistory.com/132
### 컴퓨터 네트워크

*  OSI Layer 1 관련 개념
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
      
* layer 1 정리 결론
  *  네트워크가 초기에 구성될때의 모습이다. IP 프로토콜이 만들어지기 이전의 네트워크 구성이다.


* OSI 7 계층 요약
   * https://chatgpt.com/s/t_68a7c2a6f4a081918b533658634c9c08
   * Just a Fact: 단말기 사이에 통신은 MAC adress를 사용 하여 통신한다. ARP가 단말기 사이 MAC 주소를 서로 알려주는 기능을 담담한다.

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
      *  root 유저 비밀번호 변경 참고:[URL](https://studyforus.tistory.com/223)
    
   *  내장된 방화벽 추축하기
   *  시스템 로그 구성하기
   *  고급 보안 기능
      * 보안 강화 리눅스(SELinux)
      
   *  패키지 설치 명령어
      * apt-get install [패키지명]
   *  디스크 공간 체크 명령어
      * df -h --total
   *  그 외 [Linux man pages](https://linux.die.net/man/) 참고
   
   * 로그 기록 작업: [참고](http://blog.naver.com/PostView.nhn?blogId=innerbus_co&logNo=221439737250&parentCategoryNo=&categoryNo=11&viewDate=&isShowPopularPosts=true&from=search)
   
   
   * 백업 작업: [참고](https://mamya.tistory.com/224)  
   * vim
      *  copy & paste: [참고](https://vim.fandom.com/wiki/Copy,_cut_and_paste)
   * history 명령어 실행: [보기](https://unix.stackexchange.com/questions/275053/is-there-any-way-to-execute-commands-from-history)
*  centOs
   *  about CentOs
      *  레드헷 제휴로 개발한 커뮤터 운영체제이다. 무료 기업용 컴퓨팅 플랫폼을 제공할 목적으로 만들어진 리눅스계 운영 체제 가운데 하나이다.
      *  레드헷 엔터프라이즈 리눅스의 소스 코드를 그대로 가져와 빌드해 내놓으며 이과정에서 이루어지는 변형은 레드헷의 상표가 잘리고 그자리에 CentOS의 상표가 붙는(상표권 분쟁을 피하기 위해)
      정도뿐이다.
      *  [공식 웹사이트](https://www.centos.org/)
      *  [CentOS 다운로드](https://www.centos.org/download/)
      
*  데비안과 레드헷 엔터프라이즈 리눅스 또는 페도라 시스템의 차이점
   *  리눅스 설치 과정은 복잡하다. 우분트는 이러한 설치과정을 보편적인 사용자가 수용할 수 있는 부분만 제외하고 나머지는 자동화해 놓음으로써 몇 번을 클릭만으로 설치가 가능하다.
      레드헷 시스템의 경우에는 사용자에게 워크스테이션 도는 서버, 설치할 개별 패키지 선택, 그리고 설정 옵션등 많은 설치 옵션을 제공한다.
   *  소프트웨어 관리 툴
      *  데비안: APT(Advanced Package Tool): 설치, 사제, 질의 업데이트 기능 사용
      *  레드헷: RPM
   *  GUI 툴이나 드롭다운 메뉴에서의 이들의 위치 등은 완전히 다르다.
      


### AWS
  ## AWS EC2 (생성, 연결, 보안그룹 설정) 실습  
  
  *  VPC(Virtual Private Cloud): AWS에서 제공하는 가상 컴퓨팅(네트워크) 경이다.  
  참고: [AWS VPC란 무엇입니까?](https://docs.aws.amazon.com/ko_kr/vpc/latest/userguide/what-is-amazon-vpc.html)
  
  *  Region: VPC가 생성될 지리적 위치이다. 필자는 ap-northeast-1으로 설정하였다.  
  참고: 리젼마다 서비스 제약이 있을수 있다.
  
  *  IAM(Identity and Access Management) 에서 aws console 로그인 권한 정책을 설정할 수 잇다.  
  
 
![86869060-d4ad8300-c110-11ea-89cf-d4aea65b0f4c](https://user-images.githubusercontent.com/12722674/87238560-d8a61180-c43e-11ea-8282-de3f01fd2ddd.png)

  
  
  1.  루트 사용자로 콘솔에 로그인한다
  
  1.  EC2 인스턴스(RedHet, t2.micro)를 생성해 보겠다.  
  
  ![2020-07-07 11_02_47-인스턴스 _ EC2 Management Console - Chrome](https://user-images.githubusercontent.com/12722674/86688864-706fbe00-c041-11ea-89b6-628957ae09d5.png)  

  키 페어를 생성한다.  
  참고: 키 페어란 public_key로서 AWS EC2에 로그인할떄의 필요한 공개키이다.  
  
  ![86689479-fbe94f00-c041-11ea-8a63-9afd6e7fcd46](https://user-images.githubusercontent.com/12722674/87238579-30447d00-c43f-11ea-993b-780313de20c2.png)


  인스턴스가 특정한 아이디로 등록되었으며 생성중이다.  
  
 ![86690356-d01a9900-c042-11ea-9eba-91b745daf208](https://user-images.githubusercontent.com/12722674/87238585-4eaa7880-c43f-11ea-81a8-2178ff6935f7.png)


  putty로 SSH 접속 시도해 보겠다.
  -  실패:[원인 참고](https://stackoverflow.com/questions/3190667/convert-pem-to-ppk-file-format) 
  -  puttygen을 설치 한다. [참고](https://devops.ionos.com/tutorials/use-ssh-keys-with-putty-on-windows/)  
  ![2020-07-07 12_05_03-ec2-user@ip-172-31-14-114_~](https://user-images.githubusercontent.com/12722674/86698285-22ab8380-c04a-11ea-93f1-344c8f68c60a.png)

  -  redhet ec2에 로그인 성공  
  ![86698423-4078e880-c04a-11ea-8856-feff4e508fcd](https://user-images.githubusercontent.com/12722674/87238602-887b7f00-c43f-11ea-9408-caadeb6d155d.png)

 ## Github actions를 통한 CI/CD 구축 (수정요망)
  - 배포 환경: AWS elastic beansstalk, docker
  1. `npx create-react-app` 으로 샘플 보일러플레이트 앱을 만든다.
  2. Dockerfile을 만든다.
  
  ```
FROM node:16
WORKDIR '/app'
COPY package.json ./
RUN npm install
COPY . .
RUN npm run build

#FROM nginx
#COPY --from=0 /app/build /usr/share/nginx/html
  ```
  3. github에 레포지토리를 만든다
  4. aws elastic beanstalk에 환경을 구축한다.
  5. github 마스터 브렌치에 푸시한다.
  6. github actions에 워크플로우를 세팅한다.
 
```
    name: Deployment From Github To AWS
on:
  push:
    branches:
      - master
jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Latest Repo
        uses: actions/checkout@master
        
      - name: Generate Deployment Package 
        run: zip -r deploy.zip * -x "**node_modules**"
        
      - name: Get timestamp
        uses: gerred/actions/current-time@master
        id: current-time
        
      - name: Run string replace
        uses: frabert/replace-string-action@master
        id: format-time
        with:
          pattern: '[:\.]+'
          string: "${{ steps.current-time.outputs.time }}"
          replace-with: '-'
          flags: 'g'
          
      - name: Deploy to EB
        uses: k89jy/beanstalk-deploy@v18

        with:
          aws_access_key: ${{ secrets.AWS_ACCESS_KEY_ID }}
          aws_secret_key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
          application_name: simple-engineer-deployment-tutorial
          environment_name: SimpleEngineerDeploymentTutorial-env
          version_label: "the-simple-engineer-deployment-${{ steps.format-time.outputs.replaced }}"
          region: ap-northeast-1
          deployment_package: deploy.zip
 ```
   6. github settings 에서 AWS_ACCESS_KEY_ID와 AWS_SECRET_ACCESS_KEY를 등록한다.
   7. 세팅을 완료한다.
   8. 코드를 마스터 브랜치에 푸시하면 CI/CD가 실행된다.
# DataBase softwares

## DataBase types

### Relational Databases:
     *  MySQL, Oracle, PostgreSQL, SQLite, SQL Server, Sybase, OpenEdge SQL
### Key-value stores:
     *  Berkeley DB, memcached, redis
### Document oriented Stores:
     *  couchDB, mongoDB
### Graph DataBases:
     *  Neo4j, AWS Neptune, Sesame, AllegroGraph, different RDF/triplestores


  *   RDS(Relational DataBase Service)
      *  rds 생성  
     ![86885766-cb341300-c130-11ea-88db-2099f9535f5f](https://user-images.githubusercontent.com/12722674/87238591-6da90a80-c43f-11ea-954c-77668705c951.png)

      *  rds 암호 생성  
      ![86885838-e7d04b00-c130-11ea-93c3-3a13c39c3739](https://user-images.githubusercontent.com/12722674/87238633-17889700-c440-11ea-9f6b-1b237288018d.png)

      *  다중 A-Z(마스터 슬래이브 구조이다, 프리티어 버젼에서는 제공되지 않는다)  
      ![86885964-1f3ef780-c131-11ea-9cd2-90c8978739f9](https://user-images.githubusercontent.com/12722674/87238665-836aff80-c440-11ea-8d9e-146b4579254f.png)

      
  *   Nosql vs MySql:[참고](https://siyoon210.tistory.com/130)
      
      *  MySql 1:1, 1:n, n:m 구조 설명: [참고](https://victorydntmd.tistory.com/30)
      *  MySql ACID 설명: [참고](https://victorydntmd.tistory.com/129)
   
  *  MySql vs graphDB:[참고](https://liz09045.tistory.com/142)
  *  MySql vs redis:[참고](https://m1nomi.tistory.com/25)
      
 *   Neo4j 설치 과정: [참고](https://1004jonghee.tistory.com/entry/Neo4j-Desktop-%EC%84%A4%EC%B9%98)
 
 *   MongoDB
 
     * 설치 과정  
       cmd 에서 mogoDB 실행하기
      
     * 완료 cmd log  
       ![mongodb](https://user-images.githubusercontent.com/12722674/90360838-af108380-e097-11ea-8eac-bfe33eb3b1fc.PNG)


### Node Js
  *  설치 과정
     *  [node js 다운로드](https://nodejs.org/ko/download/)  
      ![86677033-2f25e100-c036-11ea-9d83-064e700a54f0](https://user-images.githubusercontent.com/12722674/87238613-bcef3b00-c43f-11ea-91bd-c4e5f70860d2.png)
      
     *  설치 확인 명령어: `node -v`  
     
     ![2020-07-07 09_44_15-명령 프롬프트](https://user-images.githubusercontent.com/12722674/86677341-790ec700-c036-11ea-806d-cc781812e8fd.png)
     
     현제 필자의 컴퓨터에는 12.13.0 버젼이 설치되어있다.
     
     * 웹 프레임 워크인 express를 설치해 보겠다.
       *  `npm init` 을 통해 초기화 한다.  
           ![86899441-f6286200-c144-11ea-9105-f1d175d53d1e](https://user-images.githubusercontent.com/12722674/87238621-e5773500-c43f-11ea-8c71-65c18924bf69.png)
 
          package.json 파일
       *  `npm install expresss --save` 을 통해 express를 설치한다.
       *  다음 프로세스: [참고](https://www.deok.me/entry/NodeJS-NodeJS-Express-%EC%84%A4%EC%B9%98-%EB%B0%8F-%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B0%9C%EB%B0%9C-%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0)
     * express 폴더 구조 
       * `npm install -g express-generator`  
       *   `express` 명령어를 통해 folder 구조를 잡는다.
       *  미들웨어 작성: [참고](https://expressjs.com/ko/guide/using-middleware.html)  
       *  html 파일 랜더링: [참고](http://jeonghwan-kim.github.io/express-js-3-%ED%85%9C%ED%94%8C%EB%A6%BFjade/)
       *  라우터 파일  
       `res.render('[파일명].html`, [json 포맷]'
       *  app.js 파일 코드  
      ` app.use(express.static('views'));`  
       `app.use(express.static(path.join(__dirname, 'public/html')));`  
       `app.set('views', path.join(__dirname, '/views'));`  
`app.engine('html', ejs.renderFile);`  
`app.set('view engine', 'ejs');`  
## hoisting in javascript
hoisting

1. 변수 선언이 함수 맨 위로 간다
 예시 코드 ))
```
var a = "first"
var b = "second"
var c = "third"

console.log(d)

var d;
```


추측 된 결과: reference error
실제 결과 : undefined
```
var a = "first"
var b = "second"
var c = "third"

d = "fourth"

console.log(d)

var d;
```
실제 결과 : fourth

이런 현상을 hoisiting이라고 한다

hoisiting의 단점:

browser의 성능을 떨어뜨린다.

## var vs let vs const


var 는 중복 선언이 가능하다

let은 중복 선언이 불가능 하므로 var를 권장하지 않는다

const 최초의 할당한 데이터를 변경 할수 없다(상수 선언)

### python
  *  파이썬3 설치
     
     *   `sudo apt-get install python` 
  
  *  파이썬 버전(설치) 확인    
     *   `python3 --version`
 
  *  파이썬 실행  
     *   `python3`
   
  * 어떤 라이브러리가 설치되어 있는지 확인하기
    *   pip list
    
### PostMan

   * 포스트맨 다운로드 [다운로드 링크](https://www.postman.com/downloads/)

### MySql Workbench

  *  rds접속을 위해 client용으로 mySql Workbench를 사용해 보겠다.
     

### github
  * git pull vs git clone [참고](https://stackoverflow.com/questions/3620633/what-is-the-difference-between-pull-and-clone-in-git)

### Anaconda

### Juypeter noteBook

### Docker

   

   * Ubuntu에서 docker 설치 
       * 구버전 삭제  
     
     `$ sudo apt-get remove docker docker-engine docker.io containerd runc$ `  
     
       * Docker repositroy를 설치 한다
        `sudo apt-get install \
        apt-transport-https \
        ca-certificates \
        curl \
        gnupg-agent \
        software-properties-common`  
    
      * Docker 공식 GPG키를 설치 한다.  
    
      `$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`  
    
      * 키 finger print가 있는지 검색한다  
    `$ sudo apt-key fingerprint 0EBFCD88`  
      *  안정적인 repository를 셋업한다
    ` sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"`  
   
   * Docker 를 설치 한다
   
   `sudo apt-get install docker-ce docker-ce-cli containerd.io`
   
     * Docker 엔진이 설치 되어 있는지 확인한다  
   
   `sudo docker run hello-world`
   
   * Docker ngnix 설치 실습 [참고]:(https://minimilab.tistory.com/8)
   
      ***  
   ![ngxnix](https://user-images.githubusercontent.com/12722674/90309683-89636d00-df25-11ea-9c17-3861e1a03412.PNG)  
   
   * docker 프로세스 확인  
     `docker -ps`
   * docker 프로세스 삭제  
     `docker rm [container-id]`
   * docker 이미지 삭제
     `docker rmi [이미지 이름]` 
   * docker 파일 build
     `docker build [OPTIONS] PATH | URL | -`
     
     
### Slack

   *  협업 도구인 slack 사용법을 알아보자  
          
  [slack 링크](https://slack.com/intl/en-kr/)
  
   *  [ 다운로드](https://slack.com/intl/en-kr/downloads/windows)
### Trello

   *   협업 도구인 Trello 사용법을 알아보자  
   
   [Trello 링크](https://trello.com/?&aceid=&adposition=&adgroup=105703216008&campaign=9843285496&creative=437184392125&device=c&keyword=%2Btrello&matchtype=b&network=g&placement=&ds_kids=p53016482385&ds_e=GOOGLE&ds_eid=700000001557344&ds_e1=GOOGLE&gclid=Cj0KCQjw3ZX4BRDmARIsAFYh7ZKwFUSDuqnxqn_binH58nRGZ8kuIiJWJUMzUtjGJ8YBDesJJePC9m0aAtxaEALw_wcB&gclsrc=aw.ds)


### 성능 개선 방법
https://chatgpt.com/s/t_68abca8a6af48191acaae03c7213d271
