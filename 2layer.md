## 2계층

### 1) 2계층에서 하는 일

하나의 네트워크 상에 존재하는 여러 장비들 중에서 특정 장비가 어떤 장비에게 보내는 데이터를 전달한다.
추가적으로 오류 제어, 흐름제어를 수행한다.

2계층은 하나의 네트워크 대역 (LAN)에서만 통신할때 사용한다.
다른 네트워크와 통신할때는 항상 3계층이 도와주어야 된다.


### 2) 2계층에서 사용하는 주소

MAC주소 : 물리적인 주소
16진수로 이루어져 있다.
XX - XX -XX - XX -XX -XX 
이런식으로 이뤄져 있다.
앞 6자리는 제조회사 식별 ID와 뒤에 6자리는 제조사에서 부여한 고유번호가 포함되어 있다.

### 3) 2계층의 프로토콜
목적지 주소(MAC주소) , 보내는 주소 (MAC주소) , ethenet type (뒤의 페이로드가 어떤 프로토콜이 캡슐링이 된 것인지 알려주기 위함),  그리고 페이로드가 들어가게 된다.
