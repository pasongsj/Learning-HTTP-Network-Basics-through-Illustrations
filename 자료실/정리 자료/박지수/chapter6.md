# 6.6 엔티티 헤더 필드
리퀘스트, 리스폰스 모두에 사용되는 헤더필드.
엔티티에 관한 정보를 포함함.

## 6.6.1 Allow
`Allow : GET, HEAD`
서버가 받을 수 없는 메서드를 수신한 경우, 405 Method Not Allowed 리스폰스와 함게 수신 가능한 메소드의 일람을 전달함.

## 6.6.2 Content-Encoding
`Content-Encoding:gzip`
서버가 엔티티 바디에 대해서 실시한 콘텐츠 코딩 형식을 전달함. 

## 6.6.3 Content-Language
`Content-Language: en`
엔티티 바디에 사용된 자연어 타입을 전달함

## 6.6.4 Content-length
`Content-length: 15000`
byte 단위의 엔티티 바디의 크기를 전달함. 인코딩 시에는 사용하지 말것

## 6.6.5 Content-Location
`Content-Location: http://www.hacer.jp`
메시지 바디에 대응하는 URI를 전달함. 요청과 다른 리소스가 반환된 경우 사용됨.

## 6.6.6 Content-MD5
메세지 바디의 변경여부를 채킹하기 위해 MD5 알고리즘에 의해 생성된 값을 전달함.
URI에 바이너리 값을 기록하지 못하기 때문에 Base64로 인코딩함.

우발적인 변동은 감지하지만, 악의적인 변동은 감지하지 못함.

## 6.6.7 Content-Range
`Content-Range: bytes 5001-10000/10000`
일부분만 response 할 때 사용합니다. 

## 6.6.8 Content-type
엔티티 바디에 포함된 오브젝트의 미디어 타입 전달.

## 6.6.9 Expires
`Expires: Wed, 04 Jul 2012 08:26:05 GMT`
리소스 유효기간을 전달합니다.

## 6.6.10 Last Modified
`Last-Modified: Wed, 23 MAy 2012 09?59:55 GMT`
리소스가 마지막으로 갱신된 시간 전송


