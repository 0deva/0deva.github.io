---
layout: post
title: "Bubble Sort"
date: 2022-11-29 12:55:09 +0900
categories: jekyll update
comments: true
---

>## 버블 정렬 알고리즘이란?
>
>- 서로 인접한 두 원소를 검사하여 정렬하는 알고리즘 
>- 시간 복잡도가 __O(n^2)__ 로 상당히 느리지만, 코드가 단순하기 때문에 자주 사용



## 알고리즘
1. 배열의 ``두 수 (a, b)를 선택``
2. 만약 그 두 수가 정렬되었다면 놔두고 아니라면 ``두 수를 바꾸는 방식으로 진행``
3. 오름차순으로 정렬할 때는 a < b, 내림차순이라면 a > b여야 ``정렬된 것으로 판단``
4. 배열의 ``처음부터 끝까지 반복``
5. 위 알고리즘을 ``아무 변화가 없을 때까지 반복``



## Python Code
```python
def bubbleSort(x):
	length = len(x)-1
	for i in range(length):
		for j in range(length-i):
			if x[j] > x[j+1]:
				x[j], x[j+1] = x[j+1], x[j]
	return x
```

[참조링크](https://ko.wikipedia.org/wiki/%EB%B2%84%EB%B8%94_%EC%A0%95%EB%A0%AC)
