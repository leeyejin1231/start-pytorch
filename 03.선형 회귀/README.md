### 예제
- 01 [선형회귀](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-01%20%EC%84%A0%ED%98%95%ED%9A%8C%EA%B7%80.ipynb)
- 02 [자동미분](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-02%20%EC%9E%90%EB%8F%99%20%EB%AF%B8%EB%B6%84.ipynb)
- 03 [다중 선형 회귀](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-03%20%EB%8B%A4%EC%A4%91%20%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80.ipynb)
- 04 [nn.Module로 구하는 선형 회귀](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-04%20nn.Module%EB%A1%9C%20%EA%B5%AC%ED%95%98%EB%8A%94%20%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80.ipynb)
- 05 [클래스로 파이토치 모델 구현하기](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-05%20%ED%81%B4%EB%9E%98%EC%8A%A4%EB%A1%9C%20%ED%8C%8C%EC%9D%B4%ED%86%A0%EC%B9%98%20%EB%AA%A8%EB%8D%B8%20%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0.ipynb)
- 06 [미니 배치와 데이터 로드](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-06%20%EB%AF%B8%EB%8B%88%20%EB%B0%B0%EC%B9%98%EC%99%80%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EB%A1%9C%EB%93%9C.ipynb)
- 07 [커스텀 데이터셋](https://github.com/leeyejin1231/start-pytorch/blob/main/03.%EC%84%A0%ED%98%95%20%ED%9A%8C%EA%B7%80/03-07%20%EC%BB%A4%EC%8A%A4%ED%85%80%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EC%85%8B.ipynb)

## 선형회귀

H(x) = Wx+b  
 W 가중치
b 편향

### 1. Loss function

MSE(Mean Squared Error, 평균제곱오차) : 오차 제곱 합 평균

![Alt text](image-1.png)

### 2. Opimizer - Gradient Descent

![Alt text](image-2.png)  
loss가 가장 낮은 지점을 찾자 -> 기울기가 0
기울기가 낮은 방향으로 W update

-   기울기가 음수일 때 -> W 증가
-   기울기가 양수일 때 -> W 감소

![Alt text](image-3.png)

여기서 ɑ는 learning rate
