# 자바스크립트로 구현하는 자료구조

## 선형 자료 구조

### 01. 연결 리스트 | Linked List

#### (01) 연결리스트 구현

 연결리스트는 여러 개의 노드를 포인터로 연결하여 관리하는 구조. 노드는 데이터 영역과 포인터 영역으로 구분되어 데이터 영역은 데이터 값을 포인터 영역은 다음 노드의 주소값을 가진다.

 - 연결리스트 노드 = 데이터 영역 + 포인터 영역

#### (02) 즉시 호출 함수 표현식 | IIFE

- ``` (function(){...})(); ``` 는 즉시 호출 함수 표현식 또는 모듈 패턴이라고 하며 함수를 정의하자마자 바로 실행시키는 표현식 입니다.

- 이 구문은 라이브러리를 만들 때 기본이되는 패턴으로 많은 라이브러리들이 이 구문을 활용하고 있습니다. **비공개 변수가 없는 자바스크립트에 비공개(Private) 변수 기능을 넣어주기 때문입니다.** 

### 02. 스택 | Stack

#### (01) 스택 구현
 
 스택은 실생활에 많이 사용되는 자료 구조 중 하나로 한 쪽 방향으로만 데이터를 빼고 넣을 수 있는 자료구조입니다. 즉 하나의 입구를 가진 바구니에 접시를 쌓는다고 생각하면됩니다. 바구니에 접시를 쌓기 위해선 맨 위의 접시 위에 쌓을 수 밖에 없고 접시를 끄내고 싶으면 맨 위의 접시만 끄낼 수 있는 구조입니다.

 구분 | 설명 
--- | -----------------------------------------------------------------------
pop | 스택에서 데이터를 끄내는 것을 pop이라고 합니다.
push| 스택에 데이터를 넣는 것을 push라고 합니다.

#### (02) 스택 오버 플로우와 스택 언더플로우

구분 | 설명 
--- | ------------------------------------------------------------------------
Stack Overflow | 주어진 스택 메모리 보다 데이터를 더 넣어 발생하는 에러
Stack Underflow| 스택에 주어진 데이터보다 더 많은 데이터를 끄내려할 때 발생하는 에러

 자바스크립트의 이벤트처리 함수도 스택 구조로 처리된다. 이 부분에 대해서는 추후에 학습해보도록 한다.

 ### 03. 큐 | Queue

 #### (01) 큐 구현

 큐는 하나의 통로에 선 사람들의 줄과 같은 자료구조입니다. 한 쪽에서는 데이터가 들어가고 한 쪽에서는 데이터가 빠지는 구조입니다.

 구분     | 설명
 ------- | ---------
 enqueue | 큐에서 데이터를 맨 뒤에 넣는 동작을 enqueue라고 합니다.
 dequeue | 큐에서 앞의 데이터를 빼는 동작을 dequeue라고 합니다.

## 자료구조에 대한 고찰

### 01. 컴퓨터 공학 아키텍쳐 전반에 걸친 이해

 자료구조를 배우면서 컴퓨터 공학에서 배우는 대부분의 아키텍쳐들이 이를 바탕으로 설계되었다는 것을 알게되었다. 가령 HTML은 트리 구조를 통해 설계되었고, 상태머신이나 프레임 워크들의 라이프 사이클 로직은 그래프를 통해 설계되었다. 또한, 알고리즘을 통해 정렬하고 검색하는 기능들 대부분이 자료구조를 바탕으로 출발했다는 것을 알 수 있었다. 심지어 관계형 데이터 베이스 시스템을 설계할 때 사용하는 RED모형도 그래프를 바탕으로 출발하였다.

 사실 자료구조 자체만 가지고는 해결할 수 있는 문제가 많지는 않았다. 하지만, 어떤 자료구조를 사용했는가와 어떤 생각에서 해당 아키텍쳐가 설계되었을까 하는 생각을 해보니 어떤 문제가 발생했을 때 자료구조에서 시작하는 것은 어떨까하는 생각을 하였다.

 아직 자료구조를 활용한 개발을 진행해보진 않았다. 하지만, 이러한 관점에서 문제를 해결하는 방법을 알았다. 개발자로 성장하기 위해서는 알고리즘과 자료구조에 대해 심도깊은 고민을 종종해보자.