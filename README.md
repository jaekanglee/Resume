# 소개 

<img alt="깃헙 프로필 사진" src="https://avatars1.githubusercontent.com/u/23161645?s=460&v=4" width="200">

* 이재강
* Email : ksdy234@gmail.com

많은 것을 다시 배우고 있는 안드로이드 3년차 개발자 입니다.
개발자를 하며 현재 시기에 가장 크게 느끼고 있는 점은 
알고있던 것 보다 더 팀의 시너지가 중요하며, 내가 현재 옳다 확신하는 것은 항상
위험한 일이고, 개발자로써 개인의 욕심을 잘 조절하는 것이 중요하다는 부분입니다.
1년차에는 열정을 가지고 무작정 개발의 세계에 덤볐고,
2년차에는 내가 노력하는 만큼 더 성장할 수 있음을 배웠고,
현재 3년차에는 내가 스스로 파 놓은 함정에 빠지는 경우가 많음을 느끼고 있습니다.
좋은 개발자가 되길 희망하며 좋은 코드를 보고 , 좋은 팀원을 만나, 즐거운 개발 생활하며 계속해서 성장하고 싶습니다.

# 경력 기술

*  파비
    - 안드로이드 개발 주 담당
    - 약 3가지의 부모앱1, 위성앱2 개발
    - 부모 , 위성앱들의 각 상호연동을 위한 메인 관리 앱 - 파비캐시
    - 유머 커뮤니앱 - 파비 펀 
    - 스타일 커뮤니티 앱 - 파비 스타일
    - 근무 기간 : 2019.03 ~ 현재
    
* 테이스트 샵
    - 안드로이드 개발 주 담당
    - 쿠킹박스 서비스를 담당하는 O2O 앱
    - 근무 기간 : 2018.06 ~ 2018.12 
* 인카코커뮤니티
    - 안드로이드 / 서버 / 인사 담당
    - 리워드앱 개발 및 서버 개발
    - 인력 채용 및 팀원 관리 업무
    - 근무 기간 : 2018.10 ~ 2019.02
    
    
# 프로젝트 기술

## 파비캐시 (파비)
<img src="https://lh3.googleusercontent.com/mf8qvy8zPoyyZClPgn0FEAp1dRPFonJN0ORLHF_iWXbQK96LHKrjgO1fWgeyNaL-MLI=s360-rw" alt="파비캐시로고" width=40/>
`위성앱을 관리하는 부모앱`
`유저의 정보 통합 관리 앱`

* 파비캐시 앱의 신규 설계 및 개발, 유지보수, 추가 개발 등
* UsageStat을 수집 및 서버 전송 -  Loop Scheduling을 다루는 것이 주요 Issue
* AlarmManager, WorkManager, Service, Notification Interceptor 등 사용자 행동 데이터를 수집하여 서버에 주기적으로 전달 하는 일 
* 독자적인 스케쥴링을 계속 Loopping해야했기 떄문에 스케쥴링을 보장하는 것 이 최우선.
* User Interface를 모두 담당하는 기능.
* 파비의 모든 서비스에서 쓰일 포인트 관리 기능 - PG연동 및 결제
* 기능 별 SDK화 
* 위성앱간의 Interaction 
* 커스텀 뷰를 다루는 일이 굉장히 많았음. (폴리곤 차트 , 애니메이션 등)

* 사용 기술 
    - 언어 : Java, Kotlin
    - 라이브러리 : Rx2(java,Kotlin,Android) , Retrofit2, aac, Workmanager, androidx, MpChart
	Glide, 등
	
    - 사용 패턴 : mvvm구조를 지향
* 개발 기간 : 2019.03 ~ 2020.현재

 
## 파비 스타일 (파비)
<img src="https://inbalance.co.kr/wp-content/uploads/2019/05/ib_logo.png" alt="Inbalance logo" width=100/>
 
* 파비스타일 앱의 신규 설계 및 개발, 유지보수, 
* 주요기능 : 포스트 업로드, 다른 사람 포스트 보기, 광고 보기, 프로필 관리 , 채팅, 친구 추가 및 관리 
* 인스타와 매우 흡사한 UI
* 가장 중요한 기능으론 채팅기능이 되겠슴돠
* 비동기 채팅 기능 , 실시간을 위해 FCM과 주기적인 Api콜을 통해. 로컬 Db에서 서버와는 따로 Db관리를 함
* 사용 기술 
    - 언어 : Java
    - 라이브러리 : Rx2(java,Kotlin,Android) , Retrofit2, aac, Workmanager, androidx, MpChart
	Glide, 등
	
    - 사용 패턴 : mvvm구조를 지향

* 개발기간 : 2019.07 ~ 2019.12


## 파비 펀 (파비)
* 파비 펀 앱의 신규 설계 및 개발, 파비 캐시 내부 앱으로 추가
* 주요 기능: 유머 게시글 커뮤니티, 동영상, Url등 미디어에 대한 핸들링이 주요 이슈
* Ux에 맞게 미디어를 핸들링 하는 과정이 매우 어려움
* 다중 리사이클러뷰의 각 뷰타입 , 홀더에 동영상이 포함되는 구조이기 때문에 Memory에 대한 이슈가 떠올랐음
* 리사이클러뷰의 구조적 버그로 Memory Leak이 생김
* 라이프사이클 컨트롤 및 뷰 커스텀으로 해결을 시도함. 100% 해결하진 못했지만 90% 해결함
* 유튜브는 Iframe을 Web뷰로 핸들링해 구현함
* 사용 기술 
    - 언어 : Java, Kotlin
    - 라이브러리 : Rx2(java,Kotlin,Android), Retrofit2, aac, Workmanager, androidx, MpChart, ExoPlayer, YoutuebePlayer , Iframe ,Webview
				Glide, 등
    - 사용 패턴 : mvvm구조를 지향
* 개발 기간 : 2020.01 ~ 현재


  
## 참참참 ( 개인 )
* 금연을 보조하기 위한 앱
* Mvvm과 AAC등 스터디를 위한 토이 프로젝트 
* 사용 기술
	- 언어 Java
	- 라이브러리 : Retrofit2, Glide, AAC 등
	- 사용 패턴 : Mvvm 
* 개발 기간 : 2018.12 ~ 2019. 03

##테이스트샵 (테스스트샵)
* 쿠킹박스 구매 및 매니징 등을 관리하는 구독서비스 형 앱
* 신규 개발을 진행하며 기존의 Web기반으로 제작 된 Interface를 웹 + 앱과 연동할 수 있게 검증 및 협의
* 주요 기능 : 회원가입 및, 쿠킹박스 구매, 스케쥴 관리, 상품 소개, 결제 등
* 사용 기술
	- 언어 : Java
	- 라이브러리: Retrofit2, YotubePlayer, Supported Android 등
	- 사용 패턴 : Mvc
* 개발 기간: 2018.06 ~ 2018.12

##캐시타운 ( 인카코커뮤니케이션)
* Cpi, Cpc, Cpe등 타게팅 리워드 앱 
* 클라이언트 / 서버 동시 개발
* 주요 기능 :
	- 앱 설치 및 리워드 누적량에 대한 레벨링 시스템
	- 5개의 광고없체 Db를 서버에서 핸들링 후 타게팅에 맞춰 클라이언트에 제공
	- UsageStat의 History를 통해 사용자의 광고참여 밑 지속에 대한 경험치 관리 ( 서버 + 클라이언트 )
	- 타게팅 알고리즘은 -> 산학협력을 통해 강릉원주대개발 후 저는 연동결과값만을 핸들링 했습니다.
* 사용 기술
	- 언어 : Java, PHP
	- 라이브러리 : Volley , Retrofit2, Okhttp,Glide, Supported Android 등 CodeIgniter(PHP)
	- 사용패턴 : Mvc
* 개발 기간 : 2017.10 ~ 2018.01

##안녕,혼밥 ( 인카코 커뮤니케이션)
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

# 보유 기술 및 사용도구
## 사용가능 언어

- 주로 사용하는 언어는 Kotlin, Java 입니다.
- MVVM 패턴을 선호하며 다룹니다.
- RestFul API를 능숙하게 사용할 수 있고, Retrofit2.0 라이브러리를 사용합니다.
- Custom UI를 능숙하게 다룰수 있습니다.
- Clean Architecture을 선호 하며 다룹니다.
- 깔끔한 Base Code를 추구합니다.
- FireBase를 연동 할수있으며 클라우드메세지/ 데이터베이스 / 애널리틱스등을 능숙하게 다룹니다.
- Realm 라이브러리를 다룹니다.
- RxAndroid 라이브러리를 다룹니다.
- 코드 리뷰가 습관화 되어 있습니다.

## 패턴 / Architecture
- MVC, MVVM 패턴을 이해하며 사용합니다.

# 활동
* 2016 서울시 앱 공모전 출품, 150위 내 진입
* 온라인 커뮤니티 다수 활동 - 안드로이드 Qna방의 방장으로 활동
* 지속적인 스터디 활동 , 신입 또는 대학생 개인 멘토링 중
* 오프라인 컨퍼런스 지속적 참여 
* 블로그 (지속적으로 블로깅 중 ) / Youtube( 틈틈히 진행 중 )

# 학력
* 강원대학교 컴퓨터 정보통신 공학 전공 - 2011.03 ~ 2019.08
* 동국대학교 사범대학 부속 고등학교 이과 졸업 - 2008 ~ 2011.02

# 더 보기
* 블로그 : https://ppizil.tistory.com/
* 유튜브 : https://www.youtube.com/watch?v=niPFUHe5P2w&t=138s

# 그외 관심사
* Node Js, Firebase DB를 이용해 토이 프로젝트 및 초심자 강의를 개인적으로 준비중입니다.