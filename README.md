# KICT-RF
KICT 1-Dimensional River Flow model
# 모델 설명

대상 하천구간의 상하류 경계조건을 입력하여 구간 내 수위변화를 해석하는 1차원 하천수리모형 <br/>

현재 시점까지는 실측 유량 또는 수위값을 입력하고, 현재 시점이후는 유출해석 및 수위예측 모형 결과자료, 또는 수위-유량관계 값을 입력하여 하천홍수위 예측

# 모델 실행

실행환경: Google Colab

실행코드:Inference_KICT_RAIN_AI_525x625_github.ipynb <br/>

내용: 사전학습된 모델('.h5','.tflite') 이용하여 예측 수행 <br/>

사전학습모델 1: model-best_rec_180min_f.h5 재귀적 학습 네트워크를 이용하여 사전학습된 예측모델 <br/>

(참고: 윤성심(2022) 초단시간 강우예측을 위한 U-Net 기반 재귀적 예측 모델, 디지털콘텐츠학회논문지, Vol.23, No.12,pp.2481-2488) <br/>

사전학습모델 2: model-best_fcst_10min.tflite~model-best_fcst_180min.tflite 각 예측 선행 시점별 최적학습된 예측모델 <br/>


