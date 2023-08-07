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


