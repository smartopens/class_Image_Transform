## Image_Transform_by_HarrWavelet

선형대수학 수업에 진행한 프로젝트
(행렬들의 성질과 변환을 이용한 이미지 압축)  

### 진행 기간
2020-10-01 ~ 2020-10-14


### 프로젝트

이미지는 많은 양의 Data들을 포함하고 있습니다. 이를 원본 그대로 사용하려면 많은 비용을 소모합니다.  
그래서 Image Compression을 많이 진행하곤 합니다.   
이와 관련해 Haar Wavelet Transform기반의 이미지 데이터를 압축, 변화를 분석하는 프로젝트입니다.    


### 프로젝트 구성

- Image Compression 진행시 K값을 조절해가면서 압축률을 조정해본다. (B = Ht@A@H 에서 B의 Subsquare matrix크기 k)

- 고주파 이미지와 저주파 이미지의 K값 변동에 따른 차이 분석

- 이미지에서 low-frequency 영역, High-frequency 영역별 추출 확인

- low-frequency 추출을 계속 진행


### View

![image](https://user-images.githubusercontent.com/44837403/181671152-68569aea-69ef-4cd1-80cf-c0d9747f6b31.png)


### 결과 분석

- 우선 압축률 k가 커질수록 이미지 해상도가 줄어듭니다. 이 때에 고주파이미지가 저주파 이미지보다 다소 변화폭이 크게 보입니다.
  이는 Haar변환 과정에서 고주파 이미지가 손실율이 더 크기 때문입니다.

- 이미지 추출시 low-frequencey 영역이 대다수 차지하는 것을 확인할 수 있습니다. 또한 상하, 좌우의 Pixel 변화에 따른 모습 역시 확인할 수 있습니다.

- low-frequency 추출을 계속 진행해보았습니다. 이 방식으로도 이미지를 압축할 수 있습니다. 다만 해상도가 다소 떨어지게 됩니다.

