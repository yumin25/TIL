## DDoS 공격 (Distributed Denial of Service)

#### 분산 서비스 거부 공격

#### 많은 양의 트래픽을 순간적으로 일으켜 해당 서버를 마비시키는 공격

- [Land Attack](#land-attack-local-area-network-denial-attack)
- [TearDrop Attack](#teardrop-attack)
- [Ping of Death](#ping-of-death)
- [Smurfing](#smurfing)

* UDP Flooding
* SYN Flooding

<br>
<br>

## Land Attack (Local Area Network Denial Attack)

네트워크 패킷의 출발지 IP 주소나 Port를 임의로 변경하여 출발지와 목적지 IP주소 또는 Port를 동일하게 함으로써 자신에게 무한히 응답하게 한다. <br>
공격 대상의 자원을 소모시켜 실행 속도를 느리게 하거나 동작을 마비시켜 서비스 거부 상태에 빠지도록 하는 공격. 주로 연결지향적(3-Way Handshaking) 특징을 가지는 서비스에서 발생된다.

<br>

## TearDrop Attack

fragment & offset을 이용한 공격 <br>
offset값을 변조해 패킷 재조합 과정에서 반복되는 재요구와 수정을 통해 오류 또는 부하를 발생시켜 시스템에 장애를 발생시키는 공격.

<br>

## Ping of Death

정상적인 Ping 패킷의 크기는 최대 65535byte이다. 따라서 공격자가 그 이상의 패킷을 서버에 보내 시스템을 마비시키는 공격.

<br>

## Smurfing

IP나 ICMP의 특성을 악용해 많은 데이터를 서버에 보내 네트워크를 불능 상태로 만드는 공격. <br>
출발지 주소를 공격 대상의 IP 주소로 설정하고 해당 네트워크 라우터의 브로드캐스트 주소를 목적지로 해 외부의 ICMP Echo Reply를 발생시키면, 이는 해당 네트워크 내의 모든 컴퓨터로 전송되어 마비시킨다.
