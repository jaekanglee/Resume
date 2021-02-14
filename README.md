
# 소개 

<img alt="깃헙 프로필 사진" src="https://yt3.ggpht.com/-FzIzyLf9FlI/AAAAAAAAAAI/AAAAAAAAAAA/Z_NU8dTnI_4/s108-c-k-c0x00ffffff-no-rj-mo/photo.jpg" width="200">

* 이재강
* Email : ksdy234@gmail.com

`많은 것을 다시 배우고 있는 안드로이드 3년차 개발자 입니다.
개발자를 하며 현재 시기에 가장 크게 느끼고 있는 점은 
알고있던 것 보다 더 팀의 시너지가 중요하며, 내가 현재 옳다 확신하는 것은 항상
위험한 일이고, 개발자로써 개인의 욕심을 잘 조절하는 것이 중요하다는 부분입니다.
1년차에는 열정을 가지고 무작정 개발의 세계에 덤볐고,
2년차에는 내가 노력하는 만큼 더 성장할 수 있음을 배웠고,
현재 3년차에는 내가 스스로 파 놓은 함정에 빠지는 경우가 많음을 느끼고 있습니다.
좋은 개발자가 되길 희망하며 좋은 코드를 보고 , 좋은 팀원을 만나, 즐거운 개발 생활하며 계속해서 성장하고 싶습니다.`

# 경력 기술

*  파비
    - 메인 안드로이드 개발 담당
    - 약 3가지의 부모앱1, 위성앱2 개발
    - 부모 , 위성앱들의 각 상호연동을 위한 메인 관리 앱 - 파비캐시
    - 유머 커뮤니앱 - 파비 펀 
    - 스타일 커뮤니티 앱 - 파비 스타일
    - 근무 기간 : 2019.03 ~ 현재
    
* 테이스트 샵 
    - 메인 안드로이드 개발 담당
    - 쿠킹박스 서비스를 담당하는 O2O 앱
    - 근무 기간 : 2018.06 ~ 2018.12 

* 인카코커뮤니케이션즈 
    - 메인 (안드로이드 / 서버 ), 인사 담당
    - 리워드앱 개발 및 서버 개발
    - 인력 채용 및 팀원 관리 업무
    - 근무 기간 : 2017.10 ~ 2018.02
    
    
# 프로젝트 기술

## 파비캐시 (파비) 
<img src="https://rgo4.com/files/attach/images/411209/665/147/039/d644019dacdde6eff3f67abffcdb9c8e.jpg" alt=" 파비캐시1" width=150/><img src="https://is1-ssl.mzstatic.com/image/thumb/Purple113/v4/b3/84/53/b384531d-396f-ab6b-9849-4eb4b49eeeea/pr_source.png/300x0w.png" alt=" 파비스타일1" width=150/><img src="https://blog.pabii.co.kr/wp-content/uploads/shoppinglist.png" alt=" 파비스타일1" width=350/>

`앱의 주요 기능 명세`
* 파비캐시 앱의 신규 설계 및 개발, 유지보수, 추가 개발 등
* UsageStat을 수집 및 서버 전송 -  Loop Scheduling을 다루는 것이 주요 Issue
* 지속적 백그라운드 작업으로 UsageStat Info를 로컬 파일 기록 및 서버 전달
    - 포그라운드 서비스 작업 없이 주기적인 안정성을 가지고 사용자 데이터 수집 및 서버 전달을 보장하기 위해 NotificationListener, Alarm ,Workmanager, JobScheduling, Fcm, Rx 스케쥴링 등 다양한 시도를 진행했었음.
* 파비의 모든 서비스에서 쓰일 포인트 관리 기능 - PG연동 및 결제
* User Data를 Chart로 시각화 기능 ( 폴리곤 차트, 라인 차트 등 )
* 위성앱간의 Interaction 기능 
* 유저의 정보 통합 관리 앱
* 등
* 사용 기술 
    - 언어 : Java, Kotlin
    - 라이브러리 : Rx2(java,Kotlin,Android) , Retrofit2, aac, Workmanager, androidx, MpChart,SMS retriever
	Glide, 등
    - 사용 패턴 :Mvc + mvvm ( Mvvm ) 구조를 지향
* 개발 기간 : 2019.03 ~ 2020.09 - 서비스 중이며 지속적인 유지 보수 중
* 현재 상태 : 서비스 중, 지속적인 추가 개발 및 안정화 중. 
* 특이 사항: 
- 부모앱을 통해 반드시 위성 앱들을 컨트롤 해야 하기 때문에, 위성앱과 부모앱간의 디펜던시가 형성 되었고  그로인해 모든 기능별 모듈화고려해개발함

## 파비 스타일 (파비)
 <img src="https://some.pabii.co.kr/css/images/some/002_mockup.png" alt=" 파비스타일1" width=150/> <img src="https://image.winudf.com/v2/image1/a3IuY28ucGFiaWkuc29tZS5hb3Nfc2NyZWVuXzNfMTU4MjY5Nzk4MF8wNDE/screen-3.jpg?fakeurl=1&type=.jpg" alt="파비스타일2" width=150/> <img 
 src="https://is2-ssl.mzstatic.com/image/thumb/Purple113/v4/1e/85/35/1e853552-ca2b-18f6-3b87-339a0af74bff/pr_source.png/750x750bb.jpeg" alt="파비스타일3" width=150/>
 
`앱의 주요 기능 명세`
* 파비캐시 앱의 신규 설계 및 개발, 유지보수, 추가 개발 등
* 파비 캐시 앱을 통한 로그인 및 자체 회원 정보 관리 기능
* 인스타와 유사한 구조로 Post upload, Managing 등
* 자신의 포스팅을 광고로써 적용가능 
* UserData Tracking ( 광고 플레이시간 및 동영상 핸들링 , 각 유저 Interaction별 트래킹 )
* 실시간 채팅 서비스 ( Http / Fcm을 기반으로 함 )
* 등
* 사용 기술 
    - 언어 : Java
    - 라이브러리 : Rx2(java,Kotlin,Android) , Retrofit2, aac, Workmanager, androidx, Glide 등
    - 사용 패턴 : mvvm구조를 지향
* 개발기간 : 2019.07 ~ 2020.01
* 현재 상태 : 서비스 일시 중단 상태
* 특이 사항: 
- 실제 이미지를 다량으로 다루는 작업이다 보니, 이미지의 메모리 관련 이슈들이 많았었고, 커스텀 UI 개발이나, 비동기 기반으로 채팅을 구현해 데이터 싱크를 맞추는 작업이 굉장히 난해한 작업이었음. ( 서버와 클라이언트가 각자의 DB를 관리 하도록 함 ) 

## 파비 펀 (파비)
<img src="https://blog.pabii.co.kr/wp-content/uploads/Cash_FUN_Flow.png" width=450>

`앱의 주요 기능 명세`
* 파비캐시 앱의 신규 설계 및 개발, 유지보수, 추가 개발 등
* 최초 독자적인 앱으로 설계되었다가, 파비캐시 내부 앱으로 편성 됨
* 게시글( 이미지, 동영상, 외부 Media ) Upload, Managing
* 기본적인 커뮤니티의 기능을 모두 가지고 있음
* 자신의 포스팅을 광고로써 적용가능 
* UserData Tracking ( 광고 플레이시간 및 동영상 핸들링 , 각 유저 Interaction별 트래킹 )
* 카테고리 별 구독형 게시글 서비스
* 등
* 사용 기술 
    - 언어 : Java, Kotlin
    - 라이브러리 : Rx2(java,Kotlin,Android), Retrofit2, aac, Workmanager, androidx, ExoPlayer, YoutuebePlayer , Iframe ,Webview, Glide, 등
    - 사용 패턴 : mvvm구조를 지향
* 개발 기간 : 2020.01 ~ 현재
* 현재 상태 : 서비스 중, 지속적인 추가 개발 및 안정화 중. 
* 특이 상항: 
- 이미지와 더불어 동영상들이 추가되며, 메모리 이슈가 어마어마하게 발생하기 시작함. 과정 중 리사이클러뷰의 버그를 발견했으나 아직 이슈트래킹에 보고된 사항이나 해결 방법이 없었기 때문에 계속해서 트러블 슈팅을 하며 자체적으로 커스텀 리사이클러뷰를 핸들링함. 
- 2단(세로,가로) 구조의 모든 Holder가 동적으로 모든 미디어 허용가능한 뷰 였기 때문에 핸들링하는 데 상당히 어려움을 겪었음.

  
## 참참참 ( 개인 )
<img src="https://lh3.googleusercontent.com/e5FQ0llWiGX6qArc1r6FZHzTzwCsLd3IK8y9bfaw40ZKkSOLP02Mmu9nKNxRg4yk8Q=h150-rw" art="테이스트샵1" width=150><img src="https://lh3.googleusercontent.com/z-3gQBrymdHPCSIcslYuXnfEf9s3iLETmYj9f-tc1AgFKy0DMqqL_jnvMl4uQC3p7wE=h150-rw" art="테이스트샵1" width=150><img src="https://lh3.googleusercontent.com/u-czaudkYBIOFvImM0ykBc7kt-O6mfOPTEU1UcgHj_JEmy291CyMNQe4lhbetkmSqXYw=h150-rw" width=150>

`앱의 주요 기능 명세`
* 금연을 보조하기 위한 앱
* Mvvm과 AAC등 스터디를 위한 토이 프로젝트 
* 주요 기능: 금연 목표설정 기능 , 목표에 대한 LineChart 등
* 사용 기술
	- 언어 Java
	- 라이브러리 : Retrofit2, Glide, AAC 등
	- 사용 패턴 : Mvvm 
* 개발 기간 : 2018.12 ~ 2019. 03
* 현재 상태 : 서비스 일시 정지 - 신규 기능 추가 및 기획의 문제로 일시 중지 상태
* 특이사항: 
- 처음 MVVM과 DI, AAC 등을 학습하기 위한 학습 곡선을 겪음.

## 테이스트샵 (테스스트샵)
<img src="https://img4.androidappsapk.co/HbMhXhfNZRSppHBr4GeB883Wm8OhbK2aeeNGX7vdhNVjUss-JD-Tm3OvWswi9q9AWEcT=h768" art="테이스트샵1" width=150><img src="https://imgf.androidappsapk.co/8Kn5s0_piRgmvzgX7BcQCJTiqoz4NhWyGRHwlL50tGPT94WUOJDt4RLMz5P5HEOKhc8=h768" art="테이스트샵2" width=150><img src="https://img7.androidappsapk.co/QIJzWJj6SHBUEeWtIBqSTHzuW8hfHSJC0lfRat7jU-KbfllerJOB8hqEHgjM8K83xSo=h300" art="테이스트샵3" width=150>

`앱의 주요 기능 명세`
* 쿠킹박스 구매 및 매니징 등을 관리하는 구독서비스 형 앱
* 신규 개발을 진행하며 기존의 Web기반으로 제작 된 Interface를 웹 + 앱과 연동할 수 있게 검증 및 협의
* 회원가입 및, 쿠킹박스 구매, 스케쥴 관리, 상품 소개, 결제 등
* 사용 기술
	- 언어 : Java
	- 라이브러리: Retrofit2, YotubePlayer, Supported Android 등
	- 사용 패턴 : Mvc
* 개발 기간: 2018.06 ~ 2018.12
* 현재 상태: 서비스 중단 -> Web을 주 타겟으로 사업 변경 
* 특이 사항: 특정 페이지는 Data, View Layer가 모두 동적으로 변하는 것을 기획에서 요구했기 때문에, XML로 지정한 뷰를 사용하는 것이 아닌 오로지 모두 동적으로 코드로 뷰를 다루는 페이지를 만든 적이 있음.

## 안녕,혼밥 ( 인카코 커뮤니케이션즈)
<img src="https://image.winudf.com/v2/image/a3IuY28uaW5jYWNvLm5ld2hvbmJhcF8xX3NjcmVlbl8wXzE1Mzk0MDI2NjNfMDI1/screen-0.jpg?h=355&fakeurl=1&type=.jpg" art="안녕혼밥1" width=150><img src="https://image.winudf.com/v2/image/a3IuY28uaW5jYWNvLm5ld2hvbmJhcF8xX3NjcmVlbl8xXzE1Mzk0MDI2NjVfMDQx/screen-1.jpg?h=355&fakeurl=1&type=.jpg" art="안녕혼밥2" width=150><img src="https://image.winudf.com/v2/image/a3IuY28uaW5jYWNvLm5ld2hvbmJhcF8xX3NjcmVlbl8zXzE1Mzk0MDI2NzFfMDYw/screen-3.jpg?h=355&fakeurl=1&type=.jpg" art="강카 이미지1" width=150>

`앱의 주요 기능 명세`
* 혼밥족의 매칭 기능을 기반으로 한 앱
* 클라이언트 / 서버 동시 개발
* PHP,Java 소켓서버 , Firebase RealtimeDb를 혼용 함
* 최초 자바를 통해 소켓서버를 개발하고자 했으나, 트래픽 및 설계, 보안 등 여러가지 측면을 감당할 수 없다 판단해 Firebase로 채팅서버를 개발함
* 개발 도중 퇴사.
* 사용 기술
	- 언어 : Java , PHP, 
	- 라이브러리 : Retrofit2, FireBaseSdk, CodeIgniter(PHP), Glide, Supported Android 등
	- 사용 패턴 : Mvc
* 개발 기간 : 2018.01 ~ 2018 ~02
* 현재 상태 : 아마도 개발 단계에서 종료 된 것으로 보임


## 캐시타운(인카코 커뮤니케이션즈)
<img src="https://image.winudf.com/v2/image/a3IuY28uY2FzaHRvd24uYXBwX3NjcmVlbl8wXzE1MTYwODY3NTJfMDA5/screen-0.jpg?fakeurl=1&type=.jpg" art="캐시타운1" width=150><img src="https://image.winudf.com/v2/image/a3IuY28uY2FzaHRvd24uYXBwX3NjcmVlbl8yXzE1MTYwODY3NTVfMDc5/screen-2.jpg?fakeurl=1&type=.jpg" art="캐시타운2" width=150><img src="https://image.winudf.com/v2/image/a3IuY28uY2FzaHRvd24uYXBwX3NjcmVlbl8xXzE1MTYwODY3NTVfMDcy/screen-1.jpg?fakeurl=1&type=.jpg" art="캐시타운3" width=150>

`앱의 주요 기능 명세`
* Cpi, Cpc, Cpe등 타게팅 리워드 앱 
* 클라이언트 / 서버 동시 개발
* 앱 설치 및 리워드 누적량에 대한 레벨링 시스템
* 서버- 지속적인 스케쥴링으로 약 5개의 광고Data 제공 업체의 API 데이터를 수집해 가공 후 자체 데이터로 변경
* 5개의 광고없체 Db를 서버에서 핸들링 후 타게팅에 맞춰 클라이언트에 제공
* UsageStat의 History를 통해 사용자의 광고참여 밑 지속에 대한 경험치 관리 ( 서버 + 클라이언트 )
* 타게팅 알고리즘을 통해 사용자에게 적합한 광고 제공 ( 적합한 앱, 상품 등 )
* 타게팅 알고리즘은 -> 산학협력을 통해 강릉원주대개발 후 저는 연동결과값만을 핸들링 했습니다.
* 사용 기술
	- 언어 : Java, PHP
	- 라이브러리 : Volley , Retrofit2, Okhttp,Glide, Supported Android 등 CodeIgniter(PHP)
	- 사용패턴 : Mvc
* 개발 기간 : 2017.10 ~ 2018.02
* 현재 상태 : 서비스 중단
* 특이 사항 : 
- 안드로이드 개발은 둘째 치고, 서버 개발이 매우 서툴렀기 때문에 보안이나 DB관리, 부하면 에서 많이 부족한 점이 있었음 .

## 강카 (개인)
<img src="https://lh3.googleusercontent.com/QRVrX0Wo3tqyDF606v1uMxMP8YuuSvNREbyD3kg-qlBHgPZjOKpo2MHvKXoSXZ_Ao7U=h150-rw" art="강카 이미지1" width=150><img src="https://lh3.googleusercontent.com/60UoGGyU3awcXtUMCfWgVW6mOByGDFXG6Z7iNyVMY3J20Of0jLbCAGwZRGv1laRfSNw=h150-rw" art="강카 이미지2" width=150><img src="https://lh3.googleusercontent.com/v26gp4R0ow5JmpZU3y9UZ8lExWorbrPQA7S-7EL1AbGRdKgvLUYCofrsv5gzTLCtFyA=h150-rw" art="강카 이미지1" width=150><img src="https://lh3.googleusercontent.com/g6XcFxRDqgXe9lv1EsTwkgJ_hrNcVYVvS3tF2yp67ZQX6LUCk3NLakvrpl40RtJT3F3y=h150-rw" art="강카 이미지1" width=150>

* 강원대학교 인근의 카페의 정보를 학생들에게 제공하는 앱 
* 클라이언트 / 서버 동시 개발
* APM , Java
* 최초 안드로이드 앱 개발
* 강원대학 인근 카페의 모든 정보를 실시간으로 알려줌, 매장 구조, 메뉴, 영업시간, 후기, 검색 등
* 라즈베리 파이를 이용해 서버 직접 구축
* 사용 기술
	- 언어 : Java , PHP, 
	- 라이브러리 : HttpConnection, CodeIgniter(PHP), Glide, Supported Android 등
	- 사용 패턴 : Mvc
* 개발 기간 : 2017.06 ~ 2017.09
* 현재 상태 : DB의 수집이 어려운 이유로 서비스 중단 함 ( 업주들의 협조를 얻기가 굉장히 어려웠음. )
* 특이 사항 : 
- 최초 안드로이드 앱 개발을 진행했음.

# 보유 기술 및 사용도구
- Git, GIthub, Gitlab, Bitbuket, SourceTree, jd-Gui, Slack, Trello, Monday, OneDrive 등 
- 주로 사용하는 언어는 Kotlin, Java 입니다.
- MVVM 패턴을 지향하며 지속적인 학습 중에 있습니다.
- Rest Api 기반의 Networking 작업에 익숙합니다.
- 커스텀 뷰 또는 다양한 뷰 컴포넌트 사용에 익숙합니다.
- 코드 컨벤션을 중요시하게 생각하지만, 상황에 따라 적절한 판단을 지향합니다.
- FireBase의 서비스 사용에 익숙합니다.
- Local DB는 주로 aac의 Room을 사용합니다.
- Rx사용을 통해 스래딩 작업을 처리하는 데 익숙합니다. Function은 지속적인 학습 중 
- 오픈 소스 및 라이브러리의 사용에 익숙 합니다.

# 활동
* 2016 서울시 앱 공모전 출품, 150위 내 진입
* 온라인 커뮤니티 다수 활동 - 안드로이드 Qna방의 방장으로써 주 답변자로 활동 중 
* 지속적인 스터디 활동 , 신입 또는 대학생 개인 멘토링 중
* 오프라인 컨퍼런스 지속적 참여 
* 블로그 (지속적으로 블로깅 중 ) / Youtube( 틈틈히 진행 중 )

# 그외 경험
* 해군(병) 전산병 ( 하드웨어 유지보수 )
* 해군(하사) 법무실 보자관 ( 법무실 하드웨어 유지보수 및 보좌 업무, 법원 서기 업무 등 )
* 대학 생활 중 음악 동아리 회장 ( 약 40명 이상의 인원관리 경험 )

# 학력
* 강원대학교 컴퓨터 정보통신 공학 전공 - 2011.03 ~ 2018.08
* 동국대학교 사범대학 부속 고등학교 이과 졸업 - 2008 ~ 2011.02

# 자격증
* 정보처리기사 ( 2018.05 )

# 더 보기
* 블로그 : https://ppizil.tistory.com/
* 유튜브 : https://www.youtube.com/watch?v=niPFUHe5P2w&t=138s

# 그외 관심사
* Node Js, Firebase DB를 이용해 토이 프로젝트 및 초심자 강의를 지속적으로 준비 중에 있습니다.
* Android  Architecture , Design Pattern 과 코드 자체를 깨끗하게 작성하는 것, 근본적으로 안드로이드 각 컴포넌트의 소스트래킹등을  학습 중이며 계획 하고 있습니다.
