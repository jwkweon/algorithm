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
