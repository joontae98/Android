# Android
**안드로이드(Android)** 는 휴대 전화를 비롯한 휴대용 장치를 위한 운영 체제와 미들웨어, 사용자 인터페이스 그리고 표준 응용 프로그램(웹 브라우저, 이메일 클라이언트, 단문 메시지 서비스(SMS), MMS) 등을 포함하고 있는 소프트웨어 스택이자 모바일 운영 체제이다.    
**안드로이드**는 개발자들이 자바와 코틀린 언어로 응용 프로그램을 작성할 수 있게 하였으며, 컴파일된 바이트코드를 구동할 수 있는 런타임 라이브러리를 제공한다. 또한 안드로이드 소프트웨어 개발 키트(SDK)를 통해 응용 프로그램을 개발하는 데 필요한 각종 도구와 응용 프로그램 인터페이스(API)를 제공한다

출처: https://ko.wikipedia.org/wiki/%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C_(%EC%9A%B4%EC%98%81_%EC%B2%B4%EC%A0%9C)

## 주요 용어
* **Activity**: 사용자 인터페이스 화면을 구성하는 컴포넌트
* **Service**: 백그라운드에서 실행되는 컴포넌트. 시각적인 사용자 인터페이스를 가지지 않음
* **Intent**: 컴포넌트에 액션, 데이터 등을 전달하는 메시지 컴포넌트
* **Intent Filter**: 수신할 수 있는 인텐트를 정의하여 컴포넌트를 정의하는 역할을하는 컴포넌트
* **Broadcast Receiver**: 배터리 부족, 언어 설정 변경 등의 특정 브로드캐스트를 수신하거나 반응하는 컴포넌트. 시각적인 사용자 인터페이스를 가지지 않음
* **Content Provider**: 애플리케이션 간의 데이터 공유를 위해 표준화된 인터페이스를 제공하는 컴포넌트
* **Notification**: 사용자에게 특정 이벤트를 알리는 컴포넌트
* **Fragment**: 액티비티 내에서 독자적으로 동작할 수 있는 UI 컴포넌트
## Android Class 정리
#### Service
* onBind(): bindService()에 의해 서비스가 시작될 때 호출, Service객체와 Activity에서 통신할 때 사용.
* onCreate(): (최초에 한번) 서비스에서 가장 먼저 호출됨.
* onStartCommand(): 서비스가 호출될 때 마다 실행.
* onDestroy(): 서비스가 종료될 때 실행.
### Android Project
Chat App: https://github.com/joontae98/ChatApp   
랜덤 뽑기 앱(이건어때?): https://github.com/joontae98/how-about-app
