# netpractice
TCP/IP 통신에서의 addressing을 직접 실습해보는 과제입니다.  
아래 그림과 같은 네트워크에서 직접 통신이 가능하도록 주소값을 부여합니다.  
<img width="805" alt="image" src="https://github.com/user-attachments/assets/c59a5c50-5f57-4ab3-9e46-eebc421fe9c4" />

---
목차
1. 주요 개념
2. 평가 피드백
---

# 1. 주요 개념

1-1) MAC 주소 (Media Access Control Address)  

네트워크 인터페이스의 고유 식별자로, 48비트의 물리적 주소 앞 24비트는 제조사 식별 번호(OUI), 뒤 24비트는 제조사가 할당한 고유 번호로 구성된다. 예: 00:1A:2B:3C:4D:5E  


1-2) IP 주소 체계  

IPv4는 32비트 주소 체계로, Network ID와 Host ID로 구성됩니다. Network ID는 네트워크 그룹을 식별하고, Host ID는 해당 네트워크 내의 개별 호스트를 식별합니다. 예: 192.168.1.100  


1-3) 서브넷 마스크 (Subnet Mask)  

IP 주소에서 Network ID와 Host ID를 구분하는 역할을 한다.  1로 표시된 비트는 Network ID, 0으로 표시된 비트는 Host ID를 나타낸다. 예: 255.255.255.0 (/24)  


1-4) IPv4와 IPv6 비교  

IPv4: 32비트 주소 체계로, 약 43억 개의 주소 공간을 제공한다. 형식: 192.168.1.1  
IPv6: 128비트 주소 체계로, 거의 무한대의 주소 공간을 제공한다. 형식: 2001:0db8:85a3:0000:0000:8a2e:0370:7334  


1-5) 네트워크 장비  

라우터(Router): 서로 다른 네트워크 간의 통신을 가능하게 하는 3계층 장비로, IP 주소를 기반으로 최적의 경로를 선택해 패킷을 전달한다.  
스위치(Switch): 동일 네트워크 내에서 MAC 주소를 기반으로 패킷을 전달하는 2계층 장비이다.  


1-6) TCP/IP 통신  

TCP/IP는 인터넷의 핵심 프로토콜로, 4계층으로 구성된다:
응용 계층(HTTP, FTP, DNS 등)  
전송 계층(TCP, UDP)  
인터넷 계층(IP)  
네트워크 접근 계층(이더넷)  

TCP는 신뢰성 있는 데이터 전송을 보장하며, 3-way handshake를 통한 연결 설정과 데이터의 순서 보장, 오류 검출 등을 제공한다.  


2. 평가 피드백
<img width="975" alt="image" src="https://github.com/user-attachments/assets/7871a302-5ed6-439b-942e-9c880c00b8a2" />

