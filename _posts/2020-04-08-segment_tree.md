---
# layout: post
title: "Segment Tree (세그먼트 트리, 구간 트리)"
excerpt: "아하.."

categories: 
    - tree

---

배열의 특정 구간에 대한 쿼리를 빠르게 수행하기 위해 만들어진 자료 구조입니다.  
예를 들어, 배열 A가 있고 다음과 같은 연산을 수행해야 한다고 생각해보자.

1. 구간 start, end (start <= end)이 주어지고, A[start] + ... + A[end] 구하기
2. index 번째 수를 value로 변경하기.

1번 연산을 수행하는데 걸리는 시간은 O(N)이고, 2번 연산은 O(1)이 되고, 이를 M번 수행한다고 하면 O(NM + M) = O(NM)이 걸리게 됩니다.

$N^2$