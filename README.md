# 코테 대비 노트 

## 정렬
sort(), sorted() 에서 key를 이용한 정렬

첫번째 인자 기준 오름차순으로 정렬

ex: `arr = sorted(arr, key= lambda x : x[0])`

두번째 인자 기준 오름차순 다음 첫번째 인자 기준 오름차순 정렬

ex: `arr = sorted(arr, key= lambda x : (x[1], x[0]))`

딕셔너리 값으로 정렬 : 두번째 인자 역순

ex:
```
sorted_dict = sorted(my_dict.items(), key = lambda item: -item[1])
print(sorted_dict)
```

`reverse = True` 도 가능
    
```
sorted_dict = sorted(my_dict.items(), key = lambda item: item[1], reverse=True)
print(sorted_dict)
```


## heapq

```
hq = []
# 최소힙
for ...
    heapq.heappush(hq, val)

# 최대힙
for ...
    heapq.heappush(hq, -val)
    
# 리스트 -> 힙
heapq.heapify(list)
```

### 단수한 tip

리스트에 n개 원소 
```
[False] * n
[0] * n
```

- 문자열 내 특수 기호 제거
정규 표현식 `re.sub`을 이용해서 제거
```
import re

str_input = '...'

out = re.sub('[^A-Za-z0-9가-힣]', '', str_input)

```
