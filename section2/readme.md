# 섹션2. 스프링 핵심 원리 이해1 - 예제 만들기

생성일: 2024년 4월 6일 오후 9:03
태그: 하나로

# main

### package hello.core.member

- 회원 엔티티
    - 회원 등급 : enum Grade
    - 회원 엔티티 : class Member
- 회원 저장소
    - 회원 저장소 인터페이스 : interface MemberRepository
    - 메모리 회원 저장소 구현체 : class MemberRepositoryImpl
- 회원 서비스
    - 회원 서비스 인터페이스 : MemberService
    - 회원 서비스 구현체 : class MemberServiceImpl

### package hello.core

- 회원 도메인
    - 회원 가입 메인 : MemberApp

# test

- main에서 애플리케이션 로직으로 테스트 하는 것은 좋은 방법이 아니다.
- test에서 JUnit 테스트를 이용하는 것이 좋다.

### package hello.core

- 회원 도메인
    - 회원 가입 테스트

# 알게된 것

- hashmap
    - put
    - get
- final
    - 해당 필드를 초기화한 후에는 다른 객체로 변경할 수 없다.
- assertions
    - assertThat
    - isEqualTo

# 문제점

- 의존관계가 인터페이스 뿐만 아니라 구현까지 모두 의존하는 문제점이 있다.