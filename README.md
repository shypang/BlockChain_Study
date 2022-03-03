# 블록체인_클레이튼 스터디











## 해시 함수 (Hash Function)







* 임의의 길이의 데이터를 고정된 길이의 데이터로 매핑하는 함수

* {해시, 해시 값, 해시 코드}= 해시 함수에 의해 얻어지는 값

* 데이터를 X 해시함수를 H라고 표기할 때 해시를 H(X)로 표기







#### Rules 

1. 하나의 데이터에서 오직 단 하나의 해시가 도출

2. 임의의 데이터 X와 Y가 있을 때 

a. if X==Y then H(X) == H(Y)

b. if H(X) == H(Y) then X == Y

c. if H(X) == H(Y) then X == Y 











***









## 해시함수 (Hash Function) 예제 1



같은 함수로 다른 데이터를 해시했을 경우 

* 문자열 "hello!"를 SHA-256으로 해시한 결과는 다음과 같다. 

​        CEasdfas1234dsafyas78dy6127384dsaf

* 문자열 "hello?"를 SHA-256으로 해시한 결과는 다음과 같다. 

  B45CF64asdfy98hj189jsadf89asudfahsfda



같은 함수라도 다른  데이터를 해시할 경우 결과값이 크게 다른 것을 확인할 수 있다. 

* 두 해시 함수 모두 256 비트 길이의 해시를 생성한다.

 

***















![block_header](block_header.png)













***







## 블록체인이란? 



정보를 **블록**이라고 하는 단위로 저장하여 저장된 블록들을 체인형태로 묶은 저장기술 











![blockChain_structure](blockChain_structure.png)













****









## 블록 높이, 블록생성주기



![block_height](block_height.png)



비트코인 생성주기 10분

이더리움 생성주기 15초

클레이튼 생성주기 1초











![blockchain_network2](blockchain_network2.png)







* 자격이 있는 참여자는 블록을 제안(propose) 할 수 있음
* 블록 제안 자격은 네트워크마다 상이 (e.g. , PoW=Proof of Work 자격증명)
* 노드들은 제안자가 올바른 자격을 취득했는지, 제안된 블록이 올바른지 검증 뒤 블록을 자신의 체인에 추가
* 정족수 또는 정해진 기준을 만족하는 수의 노드가 블록을 자신의 체인에 추가하면 합의가 이뤄졌다고 판단









## 정리 : 블록체인의 성질



* 블록체인은 한명 이상의 참여자가 있는 네트워크에서 관리
* 네트워크 참여자 전원은 모든 블록을 동일한 순서로 저장하여 모두 같은 블록체인을 유지
* 자격이 있는 참여자는 블록을 제안할 수 있음: 블록 제안 자격은 네트워크마다 상이
* 블록이 체인에 추가됨 = 참여자들이 새 블록을 자신의 체인에 추가
* 따라서 새로운 블록이 체인에 추가되려면 네트워크의 합의가 필요: 합의방법은 네트워크마다 상이
  *  어느 한 주체가 단독으로 결정하는 구조가 아닌, 여러 참여자가 합의를 통해 결정하기 때문에 블록체인은 탈중앙화되어 있다고 표현
* 참여자 전원은 이전 블록들을 저장하고 있으므로 새로운 블록의 무결성을 확인가능
* 새롭게 제안되는 블록은 참여자들이 검증 및 합의할 수 있는 형태여야함 (투명성)
* 한번 쓰여진 블록은 이전의 합의를 번복할 수 있지 않는 한 변경될 수 없음 (불변성)

















