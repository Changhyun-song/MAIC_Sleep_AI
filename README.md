# MAIC_Sleep_AI

## MAIC Sleep AI Challenge 2021 IRail_IT팀의 Preprocessing 및 Model Code
## 적외선 수면 동영상을 이용한 수면 단계(Wake, Light Sleep(N1,N2), Deep Sleep(N3,REM)분류 모델을 만드는 것이 최종 목표입니다.
<br>[MAIC 홈페이지](https://maic.or.kr/ "MAIC 홈페이지 주소")</br>

### 데이터 설명
- 수면다윈검사 중 촬영된 적외선 수면 동영상과 어노테이션 파일로 이루어져 있음
- 1건의 검사는 약 6시간의 적외선 수면 동영상을 포함하고 있고, Train Dataset은 160건의 동영상으로 이루어져 있음.
- 주어진 영상을 30초 단위로 분석하여 각 시간대의 수면 단계를 예측하는 것이 최종 목표


### 파일 정보
- 00_Preprocessing.ipynb
  - 전처리 과정 & 데이터 설명
- 01_classification_CNN+LSTM_max.ipynb
  - CNN과 LSTM을 이용한 Classification Model
  - Imagenet pretrained model 사용 (efficientnet b0) + LSTM
- 01_classification_videocnn_max.ipynb
  - video CNN classification 모델을 사용
- 02_inference_CNN+LSTM_max.ipynb
  - Final Inference Model Code
- 03_final_threshold.ipynb
  - 최종 Score를 확인하기 위한 Code
