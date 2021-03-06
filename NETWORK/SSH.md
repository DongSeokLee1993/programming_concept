# SSH?

Secure Shell Protocol로 네트워크 프로토콜의 한 종류이다. 컴퓨터와 컴퓨터 간에 인터넷과 같은 Public Network를 통해 서로 통신을 할 때
**보안**을 갖춰 안전하게 통신하기 위한 프로토콜이다. SSH의 포트번호는 22번이다.(텔넷은 23번) SSH를 사용하는 예는

#### 1. 데이터 전송

예를 들어 github와 같은 원격저장소에 데이터를 push하는 것인데, 자신의 로컬컴퓨터에서 깃헙 서버로 올리기 위해 ssh를 사용하면 데이터가 업로드
된다.

#### 2. 원격 제어

AWS와 같은 클라우드 서비스를 사용할때, AWS의 인스턴스 서버에 접속하여 해당 머신에 명령을 내리기 위해서 SSH를 통해 접속해야 한다.

### SSH를 사용하는 이유?

Telnet 이나 FTP와 같은 프로토콜을 사용하지 않고, SSH를 사용하는 것은 다른 프로토콜 보다 보안이 뛰어나기에 사용한다.

SSH가 다른 프로토콜에 비해 보안이 뛰어난 이유는 한 쌍의 Key를 통해 인증하는 과정이 있기 때문이다. 

* Private Key

* Public Key

Pulbic Key는 공개되어도 비교적 안전한 Key 로, Public Key를 통해 메시지를 전송하기 전에 암호화를 한다. 다만 복호화는 할 수 없다.

Private Key는 절대로 외부에 노출되어선 안되는 Key로 본인의 컴퓨터 내부에 저장하게 되어있다. 이 Private Key를 통해 암호화된 메세지를 복호화
할수 있다.


#### SSH를 사용하기 위해서
windows에서 다른 컴퓨터로 접속하기 위해서 SSH를 쓰고 싶지만 어떻게 사용해야 할까?

* Powershell-OpenSSH 사용하기 : Powershell에서 ssh사용이 가능하다. 서버에 접속하기 위해 굳이 쁘띠를 설치하지 않아도 된다.

* 쁘띠(PuTTY) 사용하기 : ssh 뿐만 아니라 Telnet도 가능하다.

