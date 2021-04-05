# Ready-For-Tech-Interview :pencil2:

소프트웨어 엔지니어가 되기 위한 지식을 정리하기 위한 공간입니다.

부족한 사항, 보완할 부분을 지속적으로 업데이트해서 학습한 사항을 기록하고 로드맵을 세울 계획입니다.

jwasham의 [Coding Interview University](https://github.com/jwasham/coding-interview-university/blob/main/translations/README-ko.md#%EC%9D%B4%EA%B1%B8-%EC%99%9C-%EC%8D%A8%EC%95%BC%ED%95%98%EC%A3%A0)를 참고하고 영감을 받아 작성하고 있습니다.

## 공부한 책 목록

- [ ] 오브젝트
- [x] 객체 지향의 사실과 오해
- [ ] 클린 코드
- [ ] 실용주의 프로그래머
- [ ] 코딩 인터뷰 완전 분석
- [ ] 코드 컴플리트2
- [ ] 성공과 실패를 결정하는 1%의 네트워크 원리

## Data Structure

- ㅈ[직렬화란?](#직렬화란)
- 배열
  - 시간 복잡도
    - 접근, 수정, 배열의 끝에 삽입할 때 O(1). Index를 가지기 때문
    - 특정 위치에 삽입 / 삭제하는 경우 나머지 배열 원소들의 변동으로 인해 O(n)
  - [배열 기본 (영상)](https://www.coursera.org/lecture/data-structures/arrays-OsBSF)
- 연결 리스트
  - 시간 복잡도
    - 배열과 반대로 특정 위치에 삽입 / 삭제하는 경우 O(1)
    - 특정 위치에 접근하는 경우 O(n)
- 스택
  - FIFO의 특성, 연결 리스트와 배열로 구현이 가능합니다. 각 자료구조로 구현할 때의 장,단점을 명확히 알아야 합니다.
- 큐
- 트리
  - 트리는 노드로 이루어진 자료구조. 그래프는 트리의 한 종류이며, 일반적으로 말하는 트리는 하나의 루트 노드와 0개 이상의 자식 노드를 가지고 있다. 자식 노드 역시 0개 이상의 자식노드를 가진다.
  - 이진 트리는 각 노드가 최대 두 개의 자식을 갖는 트리를 말한다. 이진 탐색 트리는 이진 트리의 일종으로, 왼쪽 자식 노드는 부모 노드보다 작거나 같으며, 오른쪽 자식 노드는 부모 노드보다 크거나 같다.(같은 경우는 정의에 따라 달라질 수 있다)
- 그래프
  - [ ] DFS 인접 리스트로 구현하기
  - [ ] DFS 인접 행렬로 구현하기
  - [ ] BFS 인접 리스트로 구현하기
  - [ ] BFS 인접 행렬로 구현하기
- 해시 테이블

## Dynamic Programming

- [DP vs recursive implementation (영상)](https://www.coursera.org/lecture/algorithmic-thinking-2/dp-vs-recursive-implementation-M999a)

## BackTracking

- [N Queens: Backtracking (영상)](https://www.coursera.org/lecture/what-is-a-proof/n-queens-backtracking-example-optional-YiULQ)
- [ ] 백준 9663번: N-Queen 

## OS

- [교착 상태와 해결 방법](https://ko.wikipedia.org/wiki/%EA%B5%90%EC%B0%A9_%EC%83%81%ED%83%9C)

## Network

- [Access Token, Refresh Token](#token의-정의)
- [URL과 URI의 차이](#url과-uri의-차이)

## Java

- [Core: Abstract Classes and Interface (영상)](https://www.coursera.org/lecture/object-oriented-java/core-abstract-classes-and-interfaces-lc1ml)
- [Interfaces and Abstract Classes (영상)](https://www.coursera.org/lecture/java-programming-design-principles/interfaces-and-abstract-classes-dXxMO)

## Android

- [ListView와 RecyclerView의 차이](#listview와-recyclerview의-차이) 
- DP와 DPI
  - 많은 디바이스들은 각각 다른 화면 크기를 가지고 있습니다. DPI는 Dots Per Inch의 약자로, 1인치에 얼만큼의 Pixel이 들어가있는지를 나타내는 단위입니다. 각기 다른 DPI 수치를 좀 더 간단히 하기 위해 우리는 Logical DPI를 사용합니다. MDPI, XXDPI와 같은 것들입니다. 각기 다른 DPI에 동일한 UI를 보여주기 위해서는 뷰의 크기를 pixel 단위로 잡는 것보다는 DP로 잡는 것이 더 좋습니다. DP는 Density Independent Pixels로 각기 다른 DPI에 상대적인 크기를 제공합니다. MDPI에선 1dp가 1px이지만 XXDPI에서는 4px과 같은 것입니다. 이러한 DP를 사용함으로써 각기 다른 사이즈를 가진 기기에 대응할 수 있습니다.
  - [DesignBytes: Density-independent Pixels (영상)](https://www.youtube.com/watch?v=zhszwkcay2A&t=103s)

## Problem Solving

Problem Solving은 **코딩 인터뷰 완전 분석** 을 공부하면서 [Programmers](https://programmers.co.kr/learn/challenges)와 [백준](https://www.acmicpc.net/)의 문제들을 지속적으로 풀어봅니다. 맞추고 틀리고가 중요한 것이 아니라, 얼만큼 문제에 대한 정의를 잘하고 문제 해결하는 과정을 이해하고 있으며, 시간 복잡도, 공간 복잡도에 대해 이해하는지가 중요합니다.

- [ ] [멀쩡한 사각형](https://programmers.co.kr/learn/courses/30/lessons/62048)