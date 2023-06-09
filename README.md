#### 알고리즘 활용 문제풀이는 velog에 정리되어 있습니다.

# 정렬 알고리즘
## 선택 정렬
매 단계에서 가장 작은 원소를 선택해서 앞으로 보내는 정렬 방법, 앞으로 보내진 원소는 더 이상 위치 변경 X, 시간 복잡도 O(N2) 비효율적인 정렬 알고리즘
<br>
![image](https://user-images.githubusercontent.com/38232501/236789371-9a62345f-dc6b-419d-86e6-226ccaa6eabd.png)
<br>
정렬이 되어있건 되어있지 않건 많은 시간이 소모됨

## 버블 정렬
단순히 인접한 두 원소를 확인 후 정렬, 시간 복잡도 O(N2) 비효율적인 정렬 알고리즘
한번의 단계가 수행되면 가장 큰 원소가 맨 뒤로 이동, 맨 뒤로 이동한 데이터는 다음 단꼐부터 정렬에서 제외 <br>
![image](https://user-images.githubusercontent.com/38232501/236790916-4fc32f36-658d-4e4c-9697-53f62a40ce20.png)
<br>
오름차순, 내림차순 변경시에는 조건문에서 수정만 해주면 됨
선택정렬보다 더 오랜 시간이 걸림

## 삽입 정렬
시간 복잡도 O(N2)
삽입정렬을 수행할 땐 처음에 첫 번째 원소는 정렬 되어 있다고 고려, 하나씩 원소를 확인해서 어디에 들어가면 좋은지 확인
매 단계가 된 후 왼쪽에 있는 애들은 정렬이 완료

<br>

![image](https://user-images.githubusercontent.com/38232501/236792151-779a4d4a-f7aa-4191-b05a-bf3eef557bb8.png)
<br>

## 병합 정렬
시간 복잡도 (N log N), 병합정렬은 전형적인 분할 정복 (divide and conquer) 알고리즘
분할 -> 정복 -> 조합 순 

일반적으로 재귀함수를 이용하여 구현 "분할하는 방식이 동일한"경우가 많기 때문, 더 이상 쪼갤 수 없는 크기가 될 때까지 계속 분할
재귀함수를 사용하기 때문에 함수 호출 횟수가 많이 발생하여 오버헤드로 이어질 수 있음

병합정렬의 시간 복잡도는 높이가 O(log N), 너비가 O(N)인 정사각형과 유사 즉, 최악의 경우 시간 복잡도가 O(N logN)
하지만, 정복 과정에서 임시 배열이 필요하다.

<br>

![image](https://user-images.githubusercontent.com/38232501/236796557-f8c9856e-0bb8-420a-a773-3a0e3bec148e.png)

이미 두 개로 나눠진 상태에서 병합을 진행하는 과정

![image](https://user-images.githubusercontent.com/38232501/236795677-8f3b153a-eb8d-40c4-baff-40578902f9df.png)

전체진행과정

<br>

### 문자열에 대한 오름차순 정렬 예시

<br> 

![image](https://user-images.githubusercontent.com/38232501/236801433-839c81c7-96c8-4830-ad7a-720b8a001e71.png)

<br> 

### 객체에 대하여 원하는 기준으로 오름차순 정렬 예시

<br>

![image](https://user-images.githubusercontent.com/38232501/236801641-b08bbe15-182e-4f0c-9b3d-3cd174c72fba.png)

<br>

---
# 이진 탐색 
## lowerBound & upperBound

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/70701275-0222-4170-be44-897efda944b5)


<br>

---

# 백트래킹
## N-Queen

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/c42c986f-88cc-41bd-9b00-4dca5412ede8)

<br>

---

# DFS (깊이우선 탐색)


<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/3d4890f8-87ea-4f8a-9a7c-76af9eb2b0f3)


<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/845d07ad-341c-49b1-a9f3-9b1d608cb551)


<br>


---

# BFS (너비우선 탐색)

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/45b42091-d628-4d34-9a45-ec151e8894b3)


<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/48355c78-8abb-44c2-90f0-fdfca1a94b3e)

<br>

---

# 다이나믹 프로그래밍 

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/8bc20fb9-1c9d-418d-887d-ee9b102f53a9)

<br>

---

### 하향식

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/7e8ef8b8-ee05-496c-9f06-8d62552a4cd9)

<br>

---

### 상향식

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/72faa899-c1ac-4833-911e-62f56b86992c)

<br>

---


# 플로이드 워셜 알고리즘

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/fe1ca690-7a2e-4575-8c0e-bfe6b7f197a6)

<br>

![image](https://github.com/seonghyuk1/Algorithm_template/assets/38232501/49659ed0-6f9e-48d6-8ff1-bbeac30ae6b0)
