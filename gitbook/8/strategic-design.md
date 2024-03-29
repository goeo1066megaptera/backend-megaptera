# 전략적 설계 (Strategic Design)

1. Ubiquitous Language
  - DDD의 시작이자 끝
  - 도메인 전문가, 비즈니스 분석가, 소프트웨어 설계자, 프로그래머 등 모두 같은 언어를 사용한다.
    - 머릿속에 떠오르는 '개'의 이미지가 각자 다를 수는 있지만, 고양이 같은 전혀 다른 것을 떠올리지 않으면 충분함
    - 도메인 전문가의 어휘가 항상 옳은 것은 아님
    - 비즈니스 도메인을 적절히 다룰 수 있는 용어를 함께 만들어서 코드에서 사용하는 것
    - 설계하기 어렵거나 코딩하기 어려운 어휘체게는 재검토가 필요하다.
      - 이를 통해서 더 똑똑해지고, 긍정적 기술부채(도메인 지식이 더 쌓여가는)가 생김
2. Bounded Context
  - 시스템을 나누는데 사용: 소프트웨어를 조직화(Solution Space)
  - 하나의 어휘가 다양한 의미로 사용될수 있음
    - 예를 들어, Account
      - 사용자 계정
      - 은행의 통장
      - BankAccount, UserAccount 등의 prefix를 사용하면, 접두어가 넘쳐나는 상황 발생
        - 대화할때 비용이 증가
    - 맥락을 좁히면서 하나의 어휘가 하나의 대상을 지시하는 이상적 상황을 만들수 있다
    - 잘 조직화된 Bounded Context로 Ubiquitous Language를 잘 만들고 유지
3. Subdomain
  - 도메인을 나눌 때 Subdomain이라는 단위를 사용: 현실을 조직화(Problem Space)

