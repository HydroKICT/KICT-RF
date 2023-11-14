# KICT-RF
KICT 1-Dimensional River Flow model
# 모델 설명

FLDWAV 기반의 1차원 하천수리모형  
현재 시점까지는 실측 유량 또는 수위값을 입력하고, 현재 시점이후는 유출해석 및 수위예측 모형 결과자료, 또는 수위-유량관계 값을 입력하여 하천홍수위 예측

# 개발 환경

Intel Fortran

# 모델 실행

1. datafile : 입력파일명, 출력파일명, 관심지점 취약기준수위 파일명 
2. 수치해석 입력자료 : 계산시간간격, 자료수, 단면수, 상하류단 경계조건 유형, 측방유입량 개수 
3. 하천 측량자료를 이용한 단면자료 구축
4. 실측 수문자료 및 타 모형 예측자료를 이용한 상류단 경계조건, 측방유입 유량 입력
5. 하류단 경계조건으로 현재시점까지의 관측 수위값 입력, 예측수위가 없을 경우 -999.00 입력
6. 하류단 수위예측이 없을 경우, 하류단 경계조건으로 이용될 수위-유량 관계 값 입력
7. 하천 조도계수 입력 (유량별 조도계수)
8. 모형 실행 및 계산결과 확인


