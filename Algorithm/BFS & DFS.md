## BFS & DFS
<br>

- [BFS](#너비-우선-탐색-breadth-first-search) : A-B-C-D-E-F-G <br>
- [DFS](#깊이-우선-탐색-depth-first-search) : A-B-D-E-F-C-G

<img src = https://user-images.githubusercontent.com/49578987/96998920-54037d00-156f-11eb-9c0e-9a1b618f22b5.PNG width="600px">

그래프는 **Dictionary**와 **List**를 이용해 파이썬으로 표현할 수 있다.
```python
graph = dict()
graph['A'] = ['B', 'C']
graph['B'] = ['A', 'D','E','F']
graph['C'] = ['A', 'G']
graph['D'] = ['B']
graph['E'] = ['B']
graph['F'] = ['B']
graph['G'] = ['C']
```
<br><br>

## 너비 우선 탐색 (Breadth First Search)
### 루트 노드에서 시작해 같은 레벨에 있는 노드들을 먼저 탐색
<br>

**queue** 사용

```python
def bfs(graph, root):
    visited, queue = [], []
    queue.append(root)
    
    while queue:
        node = queue.pop(0)
        if node not in visited:
            visited.append(node)
            queue.extend(graph[node])
    return visited
```
실행
```python
>>> bfs(graph, A)
['A', 'B', 'C', 'D', 'E', 'F', 'G']
```
<br><br>

## 깊이 우선 탐색 (Depth First Search)

### 루트 노드에서 시작해 자식 노드들을 먼저 탐색
<br>

**queue, stack** 사용
```python
def dfs(graph, root):
    visited, stack = [], []
    stack.append(root)
    
    while stack:
        node = stack.pop()
        if node not in visited:
            visited.append(node)
            stack.extend(graph[node])
    return visited
```
실행
```python
>>> dfs(graph, A)
['A', 'C', 'G', 'B', 'F', 'E', 'D']
```