# Backend-Interview-Question

백엔드 개발자를 준비하면서 받았던 면접 질문, 학습했던 내용, 예상가능한 질문을 선별했습니다.

이 저작물은 CC BY-NC(저작자 표시-비영리)입니다.

기여를 통해서 더 좋은 컨텐츠가 될 수 있도록 해주세요.

이 컨텐츠의 목표는 가능하면 간단하게 면접질문에 대답을 할 수 있도록 하는 것입니다.

당연히 세부적인 지식에 대한 꼬리질문이 들어올 수 있으니, 깊이 있게 공부하는 것을 **권장**합니다.

신입 포지션에 대한 질문의 모음이기 때문에 경력직의 면접질문은 정리하지 않았습니다.

제가 Java를 주로 사용해서 타 언어에 대한 지식이 부족합니다. 보통 그 언어를 많이 사용해보았는지 정도의 문제가 출제됩니다. 기여가 가능하시다면 부탁드립니다.

백엔드 포지션은 면접 전 검증을 위해 과제 전형을 보는 경우도 많지만, 코딩테스트를 보는 경우가 훨씬 많습니다.

## 과제 전형

과제 전형은 애플리케이션 서버를 만들거나, 아니면 특정 프로그램을 작성하는 과제로 나눠질 수 있습니다.  
팁을 드리자면 출제 의도를 파악하려고 노력한 코딩을 하셔야합니다. 그리고, 면접에서 관련된 질문이 나올 수 있으니 사용해 본 기술이거나 처음 사용했더라도 학습을 해두셔야합니다. '왜 이 기술을 사용했는가?', '이 기술 말고 다른 선택지는 없는가?' 정도의 질문은 예상해 볼만한 질문이니 대비를 해둡시다. 과제가 통과되었다면 끝난 것이 아닙니다. 그 과제에서 더 개선할 부분은 무엇인지, 확장 포인트는 어디인지까지 고민해봅시다.

과제 전형 자체가 약간 새로운 시도에 가깝기 때문에 정답은 없습니다. 본인이 할 수 있는 최선을 다해서 해당 언어의 철학에 맞는 코드를 작성해봅시다. 가령 객체지향 프로그래밍 언어라면, '재사용성', '변경에 유연함'을 염두에 두고 개선 포인트를 잡아봅시다. 또, 해당 회사의 기술스택을 확인하고 이를 적용할만하다면 적극적으로 사용해봅시다. 최신 기술에 유연한 사고를 갖고 있다는 인상을 줄 수도 있습니다.

## 코딩테스트

코딩테스트는 여러 플랫폼이 있으며, 요즘은 프로그래머스를 많이 사용하고, 언어는 Python을 추천합니다.  
제가 추천하는 학습 방법은 2개월 정도를 잡고 코딩테스트 관련 서적을 한 권 끝내거나, 유형별 문제를 푸는 것이고, 여유가 있다면 1~2시간 풀어보고(난이도마다 상이) 풀었다면 시간 복잡도를 생각하고, 다른 풀이는 없는지 고민해봅시다. 대략 이 정도 수준의 공부를 하시고, 실력을 유지하기 위해 꾸준히 한 두 문제씩 풀어봅시다. 저는 코딩테스트가 약한편이어서 더 많은 팁을 드릴 수는 없을 것 같네요.

알고리즘 코딩테스트가 재밌다면 모르겠지만 저처럼 그리 즐겁지 않은신 분은 너무 자존심을 깎아가면서 까지 준비하지는 마시는걸 추천드립니다. 안풀리면 풀이를 보고 이해하시고, 이해가 가지 않는 문제는 현재의 나에겐 너무 어려운 문제일 뿐입니다. 나중에 다시 풀 때, 풀이 없이 풀려고 노력해보고, 같은 과정을 반복해봅시다.

실제 코딩테스트를 볼 때에는, 코드에 주석을 달아두는 편이 유용합니다. 내가 어떻게 풀려고 했는지 의도를 전달할 수 있기 때문입니다. 내가 작성한 코드를 문제와 함께 정리해둡시다. 합격한다면 어떤 질문이 나올지 생각해봅시다.

[![크리에이티브 커먼즈 라이선스](https://i.creativecommons.org/l/by-nc/2.0/kr/88x31.png)](http://creativecommons.org/licenses/by-nc/2.0/kr/)  
이 저작물은 [크리에이티브 커먼즈 저작자표시-비영리 2.0 대한민국 라이선스](http://creativecommons.org/licenses/by-nc/2.0/kr/)에 따라 이용할 수 있습니다.

## CS 관련 지식

### 네트워크

<details>
<summary>웹 통신의 큰 흐름: https://www&#46;google&#46;com/ 을 접속할 때 일어나는 일</summary>
</br>
<p>면접 단골 문제입니다. 면접관 입장에서는 한 질문으로 많은 답변을 들을 수 있기 때문에 대부분의 면접자리에서 나왔던 문제입니다.</br></br>
브라우저가 URL에 적힌 값을 파싱해서 HTTP Request Message를 만들고, OS에 전송 요청을 합니다. 이 때, Domain으로 요청을 보낼 수 없기 때문에 DNS Lookup을 수행합니다.</p>
<p>크롬의 경우 브라우저 → hosts 파일 → DNS Cache의 순서로 도메인에 매칭되는 ip를 찾습니다. 만약 없다면 루트 도메인부터 서브도메인 순으로 찾게됩니다.이 요청은 프로토콜 스택이라는 OS에 내장된 네트워크 제어용 소프트웨어에 의해 패킷에 담기고 패킷에 제어정보를 덧붙여 LAN 어댑터에 전송하고, LAN 어댑터는 이를 전기신호로 변환시켜 송출합니다.</p>
<p>패킷은 스위칭 허브 등을 경유하여 인터넷 접속용 라우터에서 ISP로 전달되고 인터넷으로 이동합니다.</br>
액세스 회선에 의해 통신사용 라우터로 운반되고 인터넷의 핵심부로 전달됩니다. 고속 라우터들 사이로 목적지까지 패킷이 흘러들어가게 됩니다.</p>
<p>핵심부를 통과한 패킷은 목적지의 LAN에 도착하고, 방화벽이 패킷을 검사한 후 캐시 서버로 보내어 웹 서버에 갈 필요가 있는지 검사합니다.</p>
<p>웹 서버에 도착한 패킷은 프로토콜 스택이 패킷을 추출하여 메시지를 복원하고 웹 서버 애플리케이션에 넘깁니다. 애플리케이션은 요청에 대한 응답 데이터를 작성하여 클라이언트로 회송하고, 이는 전달된 방식 그대로 전송됩니다.</p>
</details>

### 운영체제

### 데이터베이스

### 자료구조/알고리즘

### 암호학/보안(간단한 정도)

### 컴파일러

## 언어 관련

### Java

#### Spring/JPA

## 기타

### 디자인 패턴

### 테스트

### 인프라/클라우드

### 컨테이너

### DevOps

### 커뮤니케이션

### 최신기술에 관심이 있는지

### 웹서버의 동작과정

## 면접 꿀팁
