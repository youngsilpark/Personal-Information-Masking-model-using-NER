# NER을 활용한 한국어 개인정보 마스킹 모델

# 1. Preparing Dataset

- [AI HUB 한국어 SNS 데이터셋](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=114)

![image](https://user-images.githubusercontent.com/63226383/206382292-0cd40ad6-b885-43fd-aa7c-e2e0b0e40070.png)


## 1-1. 마스킹 카테고리 선택 및 데이터 생성 전략
 1) 이름  
  : 받침에 따라 가상 이름 생성
 2) 계정  
  : email@domain 형태의 가상 이메일 생성
 3) 신원  
  : 주민등록번호 총 13자리 (123456-12345789) , "-" 유무 고려 
 4) 번호  
  : 4자리 또는 6자리의 숫자비밀번호
 5) 전화번호    
  : 총 11자리의 전화번호, "-" 유무 고려
 6) 주소  
  : 한국에 존재하는 지명들의 무작위로 조합한 가상 주소 생성
 7) 금융정보  
  : 은행명과 계좌번호 조합

![image](https://user-images.githubusercontent.com/63226383/206383150-e8167cab-6359-42fc-87f4-a27ddb8a41bd.png)


## 1-2. 데이터 전처리 및 생성
  - 

