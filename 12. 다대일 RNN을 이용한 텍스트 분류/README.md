### 예제
- 02 [IMDB 리뷰 감성 분류하기](https://github.com/leeyejin1231/start-pytorch/blob/main/12.%20%EB%8B%A4%EB%8C%80%EC%9D%BC%20RNN%EC%9D%84%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%ED%85%8D%EC%8A%A4%ED%8A%B8%20%EB%B6%84%EB%A5%98/12-02%20IMDB%20%EB%A6%AC%EB%B7%B0%20%EA%B0%90%EC%84%B1%20%EB%B6%84%EB%A5%98%ED%95%98%EA%B8%B0.ipynb)

## 파이토치를 이용한 텍스트 분류
### 1. 훈련 데이터에 대한 이해
### 2. 훈련 데이터와 테스트 데이터
X_train, y_train  
X_text, y_text
### 3. 단어에 대한 인덱스 부여
등장 빈도수대로 단어를 정렬하여 인덱스를 부여
### 4. RNN으로 분류하기
nn.RNN(input_size, hidden_size, batch_first=True)  
input_size : 입력의 크기 (각 단어의 벡터 표현의 차원 수)  
hidden_size : 출력의 크기(output_dim)  
timesteps : 시점의 수 (각 문서에서의 단어 수)  

### 5. RNN의 다-대-일(Many-to-One) 문제


