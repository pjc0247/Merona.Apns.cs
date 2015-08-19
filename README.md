Merona.Apns.cs
====

Merona.Apns.cs는 Merona v2 스펙에 맞춰 제작됨

Merona v2
----
* Server -> Module
* 서버 프로세스당 여러개의 모듈을 장착할 수 있다.
* 서버형 모듈, internal 모듈
* 서벼형 모듈은 현재 Server 오브젝트와 동일
* internal 모듈은 프로세스 안 내부 모듈간에 통신용
* 통신할 모듈이 내부에 있던 외부에 있던 Cluster 인터페이스는 동일하게 사용 가능하며, internal 모듈간의 통신일 경우에는 소켓 대신에 공유 메세지 큐를 사용

* Machine
  * Merona Server 
    * Thread Pool
    * Modules
      * Services
        * Handlers

* Machine : 메로나 서버가 구동되는 물리/가상적 머신
* Merona Sever : 메로나 서버 프로세스
* Moudle : 큰 단위에 있어서의 기능들의 집합
* Service : 한 모듈에 있어서의 분리 가능한 기능들의 집합
* Handler : 서비스의 각 패킷들에 대한 핸들러

Merona.Apns.cs
----
* Merona에서 애플 푸시 서비스 지원을 위한 용도
* Module로 제작되기 때문에 Standalone 푸시 서버로 동작 가능
* internal 모듈로 사용되면 하나의 프로세스에 게임 서버와 푸시 서버를 함께 가지는 형태로도 가능
