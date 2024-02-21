### 힙(Heap)의 개념과 구현방법에 대해 설명하세요.

최댓값과 최솟값을 빠르게 찾을 수 있도록 고안된 완전이진트리이다.

A노드의 부모노드가 B라고 하면 A와 B는 상관관계를 가진다.

최소 힙: 부모의 키 값이 항상 작다.

최대 힙: 부모의 키 값이 항상 크다.

### 구현방법

- heapq.heappush(heap, item) : item을 heap에 추가
- heapq.heappop(heap) : heap에서 가장 작은 원소를 pop & 리턴. 비어 있는 경우 IndexError가 호출됨. 
- heapq.heapify(x) : 리스트 x를 즉각적으로 heap으로 변환함 (in linear time, O(N) )
```python
import heapq
heapq.heappush(heap, item)
heapq.heappop(heap)
heapq.heapify(l)
```