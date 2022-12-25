# 코테 대비 노트 

## 정렬
sort(), sorted() 에서 key를 이용한 정렬

첫번째 인자 기준 오름차순으로 정렬

ex: `arr = sorted(arr, key= lambda x : x[0])`

두번째 인자 기준 오름차순 다음 첫번째 인자 기준 오름차순 정렬

ex: `arr = sorted(arr, key= lambda x : (x[1], x[0]))`
