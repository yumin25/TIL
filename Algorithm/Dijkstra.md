## 다익스트라(Dijkstra) 알고리즘

하나의 정점에서 다른 모든 정점으로 가는 최단 경로를 구하는 알고리즘 중 하나.<br>
방문하지 않은 점점 중 가장 비용이 적은 정점을 방문한 후 다음 정점으로 가는 것을 고려해 해당 접점의 최소 비용을 변경 후 우선순위 큐에 넣어준다. <br>
우선순위 큐 사용 & 방문했던 노드를 재방문 하지 않는다. <br><br>
음이 아닌 가중치를 가지는 그래프만 해당한다. 음수 가중치를 포함한다면 벨만-포드 알고리즘을 사용.

- [예시](https://github.com/yumin25/algorithm/blob/master/boj/%EB%8B%A4%EC%9D%B5%EC%8A%A4%ED%8A%B8%EB%9D%BC/1753%20%EC%B5%9C%EB%8B%A8%EA%B2%BD%EB%A1%9C.java)
