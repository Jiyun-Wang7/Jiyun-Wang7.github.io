---
author: Jiyun Wang
layout: post
title: Array - Searching for items in an array (작성중)
date: 2021-04-04 00:47:00 +0900
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


if __name__ == '__main__':
    arr = [1, 2, 3, 4, 5, 6, 7, 8, 9]
    target = 9
    is_exists = linear_search(arr=arr, target=target)

```

<br><br>


## 문제풀기
---
작성중


## 관련 포스트
---
- [Array - Introduction](https://jiyun-wang7.github.io/2021-03-31/array-introduction)
- [Array - Inserting items into an array](https://jiyun-wang7.github.io/2021-04-01/array-inserting-items-into-an-array)
- [Array - Deleting items from array](https://jiyun-wang7.github.io/2021-04-02/deleting-items-from-array)


