---
author: Jiyun Wang
layout: post
title: Array - Searching for items in an array (작성중)
date: 2021-04-04 12:47:00 +0900
tags: [algorithm, data-structure]
---

## 참고
---
[https://leetcode.com/explore/learn/card/fun-with-arrays/527/searching-for-items-in-an-array/3296/](https://leetcode.com/explore/learn/card/fun-with-arrays/527/searching-for-items-in-an-array/3296/)
<br><br>

## 선형 검색 (linear Search)
---
- 인덱스를 알 수없는 경우 (대부분의 경우) Array의 모든 요소를 ​​확인해야 할 수 있다. 찾고있는 요소를 찾거나 배열의 끝에 도달 할 때까지 계속 요소를 확인한다. 즉, 모든 요소를 ​​하나씩 확인하여 요소를 찾는이 기술을 선형 검색 알고리즘이라고 한다. 
- 최악의 경우 선형 검색은 전체 Array를 확인하게 된다. 따라서 선형 검색의 시간 복잡도는 O(N) 이며, N은 배열의 길이(length)를 의미한다.

```python
from typing import List


def linear_search(arr: List[int], target: int) -> bool:
    if not arr:
        return False

    for item in arr:
        if item == target:
            return True

    return False


if __name__ == '__main__':
    arr = [1, 2, 3, 4, 5, 6, 7, 8, 9]
    target = 10
    is_exists = linear_search(arr=arr, target=target)
    print(is_exists)

```

## 이진 검색 (Binary Search)
---
- 배열의 요소가 정렬 된 순서이면 이진 검색을 사용할 수 있다. 이진 검색은 배열의 중간 요소를 반복적으로보고 찾고있는 요소가 왼쪽인지 오른쪽인지 결정한다. 
- 이 작업을 수행 할 때마다 검색해야하는 요소 수를 절반으로 줄일 수 있으므로 이진 검색이 선형 검색보다 훨씬 빠르다는 장점이 있다. 
- 이진 검색의 단점은 데이터가 정렬 된 경우에만 작동한다. 단일 검색 만 수행해야하는 경우 선형 검색보다 정렬하는 데 더 오래 걸리므로 선형 검색 만 수행하는 것이 더 빠릅니다. 많은 검색을 수행하려는 경우 반복 검색에 이진 검색을 사용할 수 있도록 데이터를 먼저 정렬하는 것이 좋다.

### 이전에 정리해둔 이진검색 (아직 문제풀이가 업데이트 되어있지 않지만, 구현은 해둠.)
- [https://jiyun-wang7.github.io/2021-03-29/binary-search](https://jiyun-wang7.github.io/2021-03-29/binary-search)

<br><br>


## 문제풀기
---
작성중


## 관련 포스트
---
- [Array - Introduction](https://jiyun-wang7.github.io/2021-03-31/array-introduction)
- [Array - Inserting items into an array](https://jiyun-wang7.github.io/2021-04-01/array-inserting-items-into-an-array)
- [Array - Deleting items from array](https://jiyun-wang7.github.io/2021-04-02/deleting-items-from-array)


