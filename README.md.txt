AndroidAysncHttpLibrary
=======================

[Korea]
안드로이드 AysncHttp 오픈소스 라이브러리 (Loopj) 1.4.7 버전을 개선한 버전 입니다.

AysncHttp 오픈소스 라이브러리는 단일 파일만 업로드가 가능합니다. 
따라서, 본 오픈소스 프로젝트를 사용하시면 단일 파일 업로드 뿐만 아니라,
다중 파일까지 업로드 하실 수 있습니다.
(정확한 사용방법은 공식홈페이지를 참조해주세요.)

공식 홈페이지 : http://loopj.com/android-async-http

[사용방법]
POST 전송시 단일 File 뿐만 아니라 File Array 형태로 다중 파일 전송이 가능합니다.

```java
RequestParams params = new RequestParams();
try {
	params.put("images[]", file);
} catch (FileNotFoundException e) {
	e.printStackTrace();
}
```


[에러 관련]
POST,GET 전송시 No valid URI scheme was provided 에러 발생시
setURLEncodingEnabled 를 비활성화 해주세요.
(URL 인코딩이 자동 활성화 되어 있기 때문에 에러 생길 수 있습니다.)


[업데이트 내역]
1. 멀티 파일 업로드 추가.


License
=======================
Apache License 2.0