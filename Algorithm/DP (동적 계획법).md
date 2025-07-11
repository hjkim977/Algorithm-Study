# 💡 DP (동적 계획법) : 다이나믹 프로그래밍
<br>

## 🎈 DP 개념
- <mark style='background-color:yellow'>**하나의 큰 문제를 여러 개의 작은 문제로 나눈 후 그 결과값을 저장하여 큰 문제를 해결할 때 사용하는 방법**</mark>
- **작은 부분들을 해결하고 이것들을 통해 전체 문제를 해결하는 방법**
<br>

## 📜 DP 사용 조건
- 큰 문제를 작은 문제로 나누었을 때 <mark style='background-color:yellow'>**동일한 작은 문제가 반복해서 등장**</mark>해야함
- 큰 문제의 해결책은 작은 문제의 해결책의 합으로 구성할 수 있어야함
<br>

## ✏️ DP로 문제 해결하는 방법
> 1. 문제를 해결하는 해가 이미 있다고 가정
> 2. 종료 조건 설정
> 3. 과정 1,2를 활용해 점화식 세우기

=> **팩토리얼 생각하기**

>Fact(N) = N!
>
>Fact(N-1) = Nx(N-1)!....
<br>

🔸점화식을 세우면,
- Fact(N) = Fact(N-1)xN (N>1)
- Fact(1) = 1           (N=1)
<br>

🔸**점화식을 어떻게 구현하면 될까?**
```python
Fact(N) :
  if (N이 1이면) 1 반환 # 종료 조건
  else Fact(N-1) * N 반환 # 일반항
```
<br>

## 🧑‍🏫 DP 방식으로 풀어야 되는 문제
- DFS/BFS로 풀 수는 있지만 경우의 수가 너무 많은 문제
- 경우의 수들에 중복적인 연산이 많은 경우
<br>

## 🚨 당부
DP는 정해져 있는 자료구조가 아니라 수행시간을 단축하는 알고리즘이기 때문에 구현 방법이 매우 많다.

그러니 문제와 풀이법을 많이 참고하자!
<br>




<출처: 코딩테스트 합격자 되기-파이썬편>
