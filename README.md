<h3>A* Pathfinding algorithm</h3>

Instead of using sorted lists, <b>heaps</b> were used. \
Reason being - A* algorithm only ever inspects and removes from one end so we can make the algorithm more efficient by using a heap.
***
<h3>What is a heap?</h3>

<h4>To quote documentation:</h4>
"Heaps are binary trees for which every parent node has a value less than or equal to any of its children."

<h5>Simple example</h5>

```
>>> def heapSort(iter):
        h = []
        for value in iter:
            heappush(h, value)
        return [heappop(h) for i in range(len(h))]

>>> heapsort([1, 3, 5, 7, 2, 4, 6, 0])
[0, 1, 2, 3, 4, 5, 6, 7]
```
