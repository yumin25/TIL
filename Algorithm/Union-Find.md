## Union-Find

서로소 집합(Disjoint Set)을 표현할 때 사용하는 알고리즘<br>

- find : 부모 값 반환
- union : 집합 합치기

1. 부모 배열에 자신을 넣기
2. x, y의 루트 노드를 찾은 뒤 y를 x의 자손으로 넣어 트리 합치기

관련 예시 : [SWEA 1251 하나로](https://github.com/yumin25/algorithm/blob/master/Swea/D4/1251%20%ED%95%98%EB%82%98%EB%A1%9C.java)
