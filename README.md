# PFALs
Plant Factory with Artificial Lighting

프로젝트를 처음 시작한 날 : 2024-11-13 (수) 오후 9시 44분.

프로젝트 목록
1. 아두이노와 온습도 센서를 사용한 데이터로거 제작. (2024-11-13)
    목표 : 저렴한 비용으로 재배환경 데이터를 실시간으로 수집, 저장할 수 있다.
    목적 : 식물공장학 실습(경북대학교 원예과학과) 과제물발표.
    
    문제인식 : 식물공장의 환경 요소 가운데 실시간으로 측정하고자 하는 요소가 있음.
     · 광환경(광도, 광질, 광주기)
      - 광도는 4개 베드별 광의 세기(PPF)를 다르게 함. 200, 250, 300, 350.
      - 광질은 4개 베드별 광도에 따른 광 스펙트럼이 거의 같은지 확인 할 필요가 있음.
      - 광주기는 공통적으로 타이머를 사용해 오전 9시에 ON, 오후 9시에 OFF됨. 명기는 12h, 암기는 12h.
     · 온도환경(주간온도, 야간온도)
      - 주야간온도는 공통적으로 오전 9시에 25℃, 오후 9시에 20℃로 설정됨.
      - 그러나 온도가 곧바로 변화하는 것은 아니기 때문에 실시간 측정이 필요함.
     · 습도환경(절대습도, 상대습도, VPD)
      - 절대습도는 공통적으로 70%로 설정하고 항상 유지함. 이를 이용하여 상대습도와 VPD를 계산할 수 있음.
     · 공기환경(이산화탄소 농도, 기류)
      - 측정하지 않음.
     · 수분환경(관수시기, 양분의 농도)
      - 동일하게 유지함.
     · 생물
      - 재배식물은 상추(Lactuca sativa) 품종 3가지.
      - 품종은 아시아종묘 로메인상추, 아진종묘 적오크상추, 경신종묘 후레쉬볼 버터헤드상추.
     질적변수는 광질, 광주기, 온도환경, 습도환경, 공기환경, 수분환경임(일정).
     양적변수는 광도 4종류, 품종 3종류임. 총 12개의 실험군이 존재.
    
    재료 : 아두이노 기판과 온습도 센서 및 부자재
     · 메인보드
      - arduino uno
     · 온습도 센서
      - DHT11
     · 상태 표시기
      - LiquidCrystal display
     · 데이터 저장 장치
      - microSD, microSD module
     · 전력 장치
      - jumper cable, on/off switch(for safety)
      - DC 1.5V AA type battery, battery holder(AA type, 6 batteries connected in series)
