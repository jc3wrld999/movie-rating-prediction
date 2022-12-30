## 미래에 볼 영화 평점 예측하기

- MovieLens 데이터 살펴보기
- 데이터 분석
    - 분석할 영화 정보 탐색하기
    - 장르의 속성 탐색
    - 분석할 유저의 정보 탐색
    - 평점 데이터 정보 탐색
    - user-movie 형태의 테이블로 살펴보기
- 수학적 기법을 이용한 평점 예측
    - SVD 를 이용한 빈칸 채우기
    - 아직 평가하지 않은 영화의 점수 예측하기
- 예측 모델 평가하기
    - 예측 모델의 평가 방법
    - 실제 평점과의 비교 시각화
    - 한걸음 더: 20대가 좋아할만한 영화를 예측
    
![image](https://user-images.githubusercontent.com/61821641/210037289-3df4a040-5e4b-4983-832b-bfbf91c6c8a9.png)

| user\_id | movie\_id | rating | time |
| --- | --- | --- | --- |
| 1 | 1193 | 5 | 978300760 |
| 1 | 661 | 3 | 978302109 |
| 1 | 914 | 3 | 978301968 |
| 1 | 3408 | 4 | 978300275 |
| 1 | 2355 | 5 | 978824291 |

| movie\_id | title | genre |
| --- | --- | --- |
| 1 | Toy Story (1995) | Animation\|Children's\|Comedy |
| 2 | Jumanji (1995) | Adventure\|Children's\|Fantasy |
| 3 | Grumpier Old Men (1995) | Comedy\|Romance |
| 4 | Waiting to Exhale (1995) | Comedy\|Drama |
| 5 | Father of the Bride Part II (1995) | Comedy |

| user\_id | gender | age | occupation | zipcode |
| --- | --- | --- | --- | --- |
| 1 | F | 1 | 10 | 48067 |
| 2 | M | 56 | 16 | 70072 |
| 3 | M | 25 | 15 | 55117 |
| 4 | M | 45 | 7 | 02460 |
| 5 | M | 25 | 20 | 55455 |

![image](https://user-images.githubusercontent.com/61821641/210037544-2017e96f-2a8d-4268-a44e-f3da3a569dc4.png)

![image](https://user-images.githubusercontent.com/61821641/210037560-ef83ebe9-ff3e-4ddc-8d1c-b268f1b883da.png)

![image](https://user-images.githubusercontent.com/61821641/210037575-744645ab-65a5-46a6-a164-72dd673e6430.png)

![image](https://user-images.githubusercontent.com/61821641/210037585-213bd8de-fb53-4776-96eb-aea0001b2b41.png)

### 각 영화의 평가 받은 횟수
![image](https://user-images.githubusercontent.com/61821641/210037595-129766bc-0a90-49e6-a3ea-48c4ca3fc025.png)

### 영화별 평균 평점
![image](https://user-images.githubusercontent.com/61821641/210037683-bb86fe0a-ea86-487e-a98f-2dc6fc61225e.png)

### 사용자 별 평가 영화 개수 분포
![image](https://user-images.githubusercontent.com/61821641/210037699-00b583cc-b8f4-4009-a478-d2488e8efbf4.png)

### 사용자 별 영화 평균 평점 분포
![image](https://user-images.githubusercontent.com/61821641/210037774-e54852f7-df0f-4d1d-ac5f-96187e10230a.png)