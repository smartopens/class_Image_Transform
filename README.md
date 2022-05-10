## Konkuk_University_ClassProject_Image_Transform

선형대수학 수업에 진행한 프로젝트입니다. 행렬들의 성질과 변환에 대해 공부했습니다.    
이를 기반으로 Image 데이터들을 압축하고 그 변화들을 분석하는 프로젝트입니다.   

## 진행 기간
2020-10-01 ~ 2020-10-14


## 프로젝트 개요

이미지는 안에 많은 Data들을 포함하고 있습니다. 고로 이를 원본 그대로 인터넷에서 사용하려면 많은 비용을 소모합니다. 그래서 Image Compression을 많이 진행하곤 합니다.   
이를 위해서 Haar Wavelet Transform에 대해서 구축해보고 Test 진행했습니다.


## 프로젝트 구성

- Image Compression 진행시 K값을 조절해가면서 압축률을 조정해본다. (B = Ht@A@H 에서 B의 Subsquare matrix크기 k)

- 고주파 이미지와 저주파 이미지의 K값 변동에 따른 차이 분석해보기

- 이미지에서 low-frequency 영역, High-frequency 영역별 추출 확인해보기

- low-frequency 추출을 계속 진행해보기


## 주요 동작 화면

![image](https://user-images.githubusercontent.com/44837403/123373030-a514b680-d5bf-11eb-9b65-a89cc52a33b5.png)



## 결과물 분석

- 우선 압축률 k가 커질수록 이미지 해상도가 줄어듭니다. 이 때에 고주파이미지가 저주파 이미지보다 다소 변화폭이 크게 보입니다.
  물론 직관적으로 고주파 이미지의 pixel의 변화가 자체적으로 많아서 그런것일 수 있지만 Haar변환 과정에서 고주파 이미지가 손실율이 더 큰 이유도 있습니다.

- 이미지 추출시 low-frequencey 영역이 대다수 차지하는 것을 확인할 수 있습니다. 또한 상하, 좌우의 Pixel 변화에 따른 모습 역시 확인할 수 있습니다.

- low-frequency 추출을 계속 진행해보았습니다. 이 방식으로도 이미지를 압축할 수 있습니다. 다만 해상도가 다소 떨어지게 됩니다.

