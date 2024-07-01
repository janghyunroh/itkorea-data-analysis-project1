# 0. 저장소 설명

it코리아 학원의 2024 데이터 분석 및 파이썬 프로그래밍 과정 1차 프로젝트 - 3조의 저장소입니다.

데이터 분석을 통해 원인을 해결할 문제를 선정한 뒤, 해당 문제의 원인에 대한 가설을 설정하고,

데이터 분석과 시각화를 통해 해당 가설을 입증 또는 반박, 새로운 가설을 제시하여 

최종적인 해결책을 제시하는 것이 목표입니다. 


# 1. 주제 선정 및 목적 설정 - 도로 교통 사고 원인 분석 및 해결 방안

일반적인 도로 교통 사고의 원인을 분석하고, 해당 원인을 제거하기 위한 해결 방안을 제시한다.

[참고 데이터]
1. 메인 데이터셋 : https://www.kaggle.com/datasets/saurabhshahane/road-traffic-accidents
2. 서브 데이터셋 : https://kosis.kr/statHtml/statHtml.do?orgId=132&tblId=DT_13204_A0400&vw_cd=MT_ZTITLE&list_id=C_6_2023_001&scrId=&seqNo=&lang_mode=ko&obj_var_id=&itm_id=&conn_path=MT_ZTITLE&path=%2FstatisticsList%2FstatisticsListIndex.do
3. 기타 데이터셋 및 뉴스 기사
    https://www.kaggle.com/datasets/jacksondivakarr/car-crash-dataset
   
    https://tmacs.kotsa.or.kr/

# 2. 가설 설정

1) 교통 사고 발생 빈도는 특정 연령대의 운전자에게 집중되어 있을 것이다.

   1 - 1) 주변 시야와 반응 속도가 떨어지는 노령 운전자의 경우에 대해 가장 높을 것이다.
   
   1 - 2) 운전 경험이 부족하여 상황 대처 능력이 떨어지는 젊은 운전자의 경우에 대해 가장 높을 것이다.

   [참고 데이터셋] 

2) "일일" 교통 사고 발생 빈도는 특정 시간대에도 집중되어 있을 것이다.
   
   2 - 1) 교통량이 큰 출퇴근 시간대에 발생 빈도가 높을 것이다.
   
   2 - 2) 시야 확보가 잘 되지 않는 야간 시간대에 발생 빈도가 가장 높을 것이다.

   [참고 데이터셋] 하루 사고 발생량 평균 분포

3) "연간" 교통 사고 발생 빈도는 특정 날짜의 기간에 집중되어 있을 것이다.
   
   3 - 1) 계절적 특성으로 인해 도로가 미끄러울 확률이 높은 11~1월 사이에 사고 발생 빈도가 높을 것이다.
   
   3 - 2) 가족, 학교 등의 단위로 체험 학습이나 여행 등을 다니는 5~7월 사이에 사고 발생 빈도가 높을 것이다.

   [참고 데이터셋] 연간 사고 발생량 분포

4) "지역에 따른" 교통 사고 발생 빈도는 특정 유형의
   
   4 - 1) 교통량이 높은 도시가 시골보다 사고 발생률이 높을 것이다. 

        4 - 1 - 1) 도시 내에서도 교통이 더 혼잡한 업무지구가 주거지구보다 사고 발생률이 더 높을 것이다. 

5) "차량의 종류에 따른" 교통 사고 발생 빈도는 특정 유형의 차량에 밀집되어 있을 것이다.
   
   5 - 1) 개인용 차량보다 공업용 차량의 사고 발생 빈도가 더 높을 것이다.

   5 - 2) 개인용 차량 중에서는 SUV가 소형 차량보다 사고 빈도가 더 높을 것이다. 
   
6) "도로 유형에 따른" 교통 사고 발생 빈도는 특정 유형의 도로에 집중되어 있을 것이다.
   
   6 - 1) 일반 국도보다 고속도로나 터널 안이 더 발생 빈도가 높을 것이다.

   6 - 2) 평지보다 오르막이나 내리막의 도로에서 더 발생 빈도가 높을 것이다.


[ 기타 생각나는 요인이 있으시면 추가 바랍니다.]

[ 여기서 유의미하고 조사해볼 가치가 있는 가설을 취사 선택하여 분석을 진행하면 좋을 것 같습니다. ]




