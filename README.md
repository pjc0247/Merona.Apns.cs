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

Merona.Apns.cs
----
* Merona에서 애플 푸시 서비스 지원을 위한 용도
* Module로 제작되기 때문에 Standalone 푸시 서버로 동작 가능
* internal 모듈로 사용되면 하나의 프로세스에 게임 서버와 푸시 서버를 함께 가지는 형태로도 가능
