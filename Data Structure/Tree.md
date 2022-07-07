## 트리 (Tree)

### 정의 : 1:n의 비선형 자료구조, 계층 관계를 가지는 계층형 자료구조

그래프의 일종이다. <br>
간선의 개수 : 정점의 개수 -1개

<br>

### 관련 용어

- 노드(node) : 트리를 구성하는 원소
- 간선 (edge) : 노드를 연결하는 선. 부모와 자식 연결.
- 루트 노드(root node) : 최상위 노드
- 단말 노드(leaf node) : 자식이 없는 노드
- 서브 트리(subtree) : 자식 노드를 최상위 노드로 하는 트리.

<br>

[이진 트리](#binary) <br>
[이진 탐색 트리](#binary_search) <br>
[포화 탐색 트리](#full) <br>
[완전 이진 트리](#complete) <br>
[편향 이진 트리](#skewed)

<br><br>

### 트리 순회 (Tree Traversal) <a id='traversal'></a>

- 전위 순회 (preorder) : 루트 - 왼쪽 - 오른쪽
- 중위 순회 (inorder) : 왼쪽 - 루트 - 오른쪽
- 후위 순회 (postorder) : 왼쪽 - 오른쪽 - 루트

<br>

### 이진 트리 (Binary Tree) <a id='binary'></a>

모든 자식 노드가 두 개 이하인 트리

<br>

### 이진 탐색 트리 (BST, Binary Search Tree) <a id='binary_search'></a>

정렬된 이진 트리. <br>
각 노드의 왼쪽 서브 트리는 해당 노드의 값보다 작은 값의 노드로만 이루어져 있다. <br>
각 노드의 오른쪽 서브 트리는 해당 노드의 값보다 큰 값의 노드로만 이루어져 있다. <br>
중복된 키 허용 X

**검색** : 루트 노드에서 시작해 노드보다 작으면 왼쪽 하위 노드, 노드보다 크면 오른쪽 하위 노드와의 비교를 반복해 일치하는 값을 찾는다. 검색 값이 없을 경우 null 반환. <br>

**삽입** : 루트 노드에서 시작해 노드보다 작으면 왼쪽 하위 노드, 노드보다 크면 오른쪽 하위 노드와의 비교를 반복한 뒤 리프 노드( 탐색 실패한 곳)에 삽입. <br>

**삭제** : 삭제할 노드 3가지 경우

1. 단말 노드 : 노드 삭제
2. 자식 노드 1개 : 노드를 삭제하고 해당 노드의 자식 노드와 부모 노드 연결
3. 자식 노드 2개 : 노드를 삭제하고 왼쪽 서브트리 중 가장 큰 값 또는 오른쪽 서브트리 중 가장 작은 값을 선택해 삭제된 노드의 위치에 이동시킨 뒤 그 노드의 자식 노드와 부모 노드를 연결시킨다.

<br>

**시간복잡도** <br>
평균 : O(𝑙𝑜𝑔N) <br>
최악의 경우 : O(N)

<br>

### 포화 이진 트리 (Full Binary Tree) <a id='full'></a>

모든 레벨에 노드가 모두 차 있는 이진 트리 <br>
노드 개수 : 2<sup>높이</sup>-1개

<br>

### 완전 이진 트리 (Complete Binary Tree) <a id='complete'></a>

단말 노드를 제외한 모든 노드가 모두 차 있으며 단말 노드는 왼쪽부터 차 있는 이진 트리

<br>

### 편향 이진 트리 (Skewed Binary Tree) <a id='skewed'></a>

최소 노드(높이+1개)의 노드를 가지면서 모든 노드가 한 방향으로만 서브 트리를 가지고 있는 트리

- 왼쪽 편향 이진 트리
- 오른쪽 편향 이진 트리